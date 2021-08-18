---
title: Включить Сейф вложения для SharePoint Online, OneDrive и Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332392"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Включить Сейф вложения для SharePoint Online, OneDrive и Microsoft Teams

1. Используя учетные данные глобального администратора или администратора безопасности, откройте портал Microsoft 365 Defender по ссылке, а затем перейдите к политикам & правил политики угрозы Сейф вложениям в разделе <https://security.microsoft.com>  \>  \>  **Политики**

   Чтобы перейти непосредственно **на страницу Сейф вложения,** используйте <https://security.microsoft.com/safeattachmentv2> .

2. На странице **Сейф вложения нажмите** **глобальные параметры**.
3. На вылете, который появится, выберите включите Microsoft Defender для Office 365 для **SharePoint, OneDrive и Microsoft Teams,** а затем выберите **Сохранить**.

    **Совет.** Сделайте следующие действия, чтобы повысить защиту Сейф вложений для SharePoint, OneDrive и Microsoft Teams:
    - Чтобы запретить пользователям скачивать вредоносные файлы, используйте значение `$true` *параметра DisallowInfectedFileDownload* в комлете **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** в SharePoint PowerShell. Дополнительные сведения см. в [SharePoint Online PowerShell, чтобы](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)запретить пользователям скачивать вредоносные файлы.
    - [Создание политики оповещения для обнаруженных файлов](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Дополнительные сведения см. [в Сейф приложения Office 365 для SharePoint, OneDrive и Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
