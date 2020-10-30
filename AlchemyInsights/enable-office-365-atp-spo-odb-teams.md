---
title: Включение пакета Office 365 ATP для SharePoint, OneDrive и Microsoft Teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801069"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="5646e-102">Включение защитника Microsoft для Office 365 для SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5646e-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="5646e-103">Перейдите на https://protection.office.com и войдите.</span><span class="sxs-lookup"><span data-stu-id="5646e-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="5646e-104">Выберите **Threat management** пункт  >  **Policy**  >  **безопасные вложения** политики управления угрозами.</span><span class="sxs-lookup"><span data-stu-id="5646e-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="5646e-105">Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams** , а затем нажмите кнопку **сохранить** .</span><span class="sxs-lookup"><span data-stu-id="5646e-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="5646e-106">Предложен В качестве глобального администратора или администратора SharePoint Online выполните командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **дисалловинфектедфиледовнлоад** , для которого задано *значение true* .</span><span class="sxs-lookup"><span data-stu-id="5646e-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="5646e-107">Предложен [Настройка оповещений](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) об обнаруженных файлах.</span><span class="sxs-lookup"><span data-stu-id="5646e-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="5646e-108">Служба ATP будет сканировать каждый отдельный файл в SharePoint Online, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5646e-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="5646e-109">Файлы сканируются асинхронно, с помощью процесса, использующего общие и гостевые события, вместе с интеллектуальными эвристиками и сигналами угроз для идентификации вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="5646e-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="5646e-110">Ознакомьтесь с разделом [ATP для SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5646e-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>