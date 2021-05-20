---
title: Включить Office 365 atP для SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543941"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="773fc-102">Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="773fc-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="773fc-103">Перейдите на https://protection.office.com и войдите.</span><span class="sxs-lookup"><span data-stu-id="773fc-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="773fc-104">Выберите **политику управления**  >    >  **угрозами Сейф вложения.**</span><span class="sxs-lookup"><span data-stu-id="773fc-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="773fc-105">Выберите **Включить Защитник для Office 365 для SharePoint, OneDrive и Microsoft Teams,** а затем нажмите **кнопку Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="773fc-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="773fc-106">(Рекомендуется) В качестве глобального администратора или администратора SharePoint Online запустите комлет [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **DisallowInfectedFileDownload,** заданным для *true*.</span><span class="sxs-lookup"><span data-stu-id="773fc-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="773fc-107">(Рекомендуется) [Настройка оповещений](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для обнаруженных файлов.</span><span class="sxs-lookup"><span data-stu-id="773fc-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="773fc-108">Microsoft Defender для Office 365 не будет сканировать каждый файл SharePoint Online, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="773fc-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="773fc-109">Файлы сканируют асинхронно, с помощью процесса, который использует события совместной и гостевой активности, а также интеллектуальные heuristics и сигналы угрозы для выявления вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="773fc-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="773fc-110">См. в Office 365 [Microsoft Defender для SharePoint, OneDrive и Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="773fc-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>