---
title: Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552522"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fa0ca-102">Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fa0ca-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="fa0ca-103">Используя учетные данные глобального администратора или администратора безопасности, войдите в Центр безопасности и соответствия требованиям [Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="fa0ca-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="fa0ca-104">Выберите **управление угрозами** в левой области, а затем выберите **вложения Policy**  >  [Safe.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="fa0ca-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="fa0ca-105">**Включите Microsoft Defender для Office 365 для SharePoint, OneDrive** и Microsoft Teams, а затем выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="fa0ca-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="fa0ca-106">В качестве глобального администратора или администратора SharePoint Online запустите следующий комдлет PowerShell с параметром **DisallowInfectedFileDownload,** заданным для *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="fa0ca-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="fa0ca-107">Настройка оповещений для обнаруженных файлов</span><span class="sxs-lookup"><span data-stu-id="fa0ca-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="fa0ca-108">Дополнительные сведения см. [в разделе Microsoft Defender for Office 365 для SharePoint, OneDrive и Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="fa0ca-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
