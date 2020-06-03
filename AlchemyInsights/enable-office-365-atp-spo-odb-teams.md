---
title: Включение пакета Office 365 ATP для SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506931"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2bd35-102">Включение расширенной защиты от угроз для Office 365 для SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2bd35-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="2bd35-103">Перейдите на https://protection.office.com и войдите.</span><span class="sxs-lookup"><span data-stu-id="2bd35-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="2bd35-104">Выберите **Threat management**пункт  >  **Policy**  >  **безопасные вложения**политики управления угрозами.</span><span class="sxs-lookup"><span data-stu-id="2bd35-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="2bd35-105">Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams**, а затем нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="2bd35-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="2bd35-106">Предложен В качестве глобального администратора или администратора SharePoint Online выполните командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **дисалловинфектедфиледовнлоад** , для которого задано *значение true*.</span><span class="sxs-lookup"><span data-stu-id="2bd35-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="2bd35-107">Предложен [Настройка оповещений](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) об обнаруженных файлах.</span><span class="sxs-lookup"><span data-stu-id="2bd35-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="2bd35-108">Служба ATP будет сканировать каждый отдельный файл в SharePoint Online, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2bd35-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="2bd35-109">Файлы сканируются асинхронно, с помощью процесса, использующего общие и гостевые события, вместе с интеллектуальными эвристиками и сигналами угроз для идентификации вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="2bd35-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="2bd35-110">Ознакомьтесь с разделом [ATP для SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2bd35-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>