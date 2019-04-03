---
title: Включение пакета Office 365 ATP для SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031070"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="a1e80-102">Включение расширенной защиты от угроз для Office 365 для SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a1e80-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="a1e80-103">Перейдите на https://protection.office.com и войдите.</span><span class="sxs-lookup"><span data-stu-id="a1e80-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="a1e80-104">Выберите пункт**безопасные вложения\*\*\*\*политики** >  **управления** > угрозами.</span><span class="sxs-lookup"><span data-stu-id="a1e80-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="a1e80-105">Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams**, а затем нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="a1e80-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="a1e80-106">Предложен В качестве глобального администратора или администратора SharePoint Online выполните командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **дисалловинфектедфиледовнлоад** , для которого задано *значение true*.</span><span class="sxs-lookup"><span data-stu-id="a1e80-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="a1e80-107">Предложен [Настройка оповещений](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) об обнаруженных файлах.</span><span class="sxs-lookup"><span data-stu-id="a1e80-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="a1e80-108">Служба ATP будет сканировать каждый отдельный файл в SharePoint Online, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a1e80-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="a1e80-109">Файлы сканируются асинхронно, с помощью процесса, использующего общие и гостевые события, вместе с интеллектуальными эвристиками и сигналами угроз для идентификации вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="a1e80-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="a1e80-110">Просмотреть [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a1e80-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>