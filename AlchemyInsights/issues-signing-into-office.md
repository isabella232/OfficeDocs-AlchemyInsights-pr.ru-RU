---
title: Проблемы с входом в Microsoft 365 приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744659"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Проблемы с входом в Приложения Microsoft 365

Примечание. Если вы используете более старую версию Windows (например, Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), используйте простое исправление, чтобы включить TLS 1.2 в качестве по умолчанию. Дополнительные сведения см. в статье [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Чтобы устранить проблемы со входом в приложения Microsoft 365, попробуйте воспользоваться следующими вариантами на затронутом компьютере.  

- Для Windows см. Рекомендации [по решению общих](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) проблем с входом
- Для Mac [см. статью Can't sign in to an Office 2016 для Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Совет**: на компьютерах с Windows можно диагностировать и автоматически устранять некоторые распространенные проблемы с входом в Office. Для использования нашего автоматического инструмента скачайте и запустите **[помощника по поддержке и восстановлению (Майкрософт)](https://aka.ms/SaRA-OfficeSignInScenario)**.

**Примечание:** Отключение современной проверки подлинности (ADAL) или управления веб-учетной записью (WAM) для устранения проблем с входом или активацией не **рекомендуется.** Если ошибки возникают при подключении к Microsoft 365 с Office 2013 [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) г., убедитесь, что вы включаете современную проверку подлинности для Office клиента.

Конкретные действия по устранению неполадок см. в.

[Проблемы с подключением при входе в систему после обновления до Office 2016, сборка 16.0.7967, на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Вы не можете войти в организационную учетную запись, например Office 365, Azure или Intune.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Устранение неполадок не браузерных приложений, которые не могут войти в Office 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Многократное запрос на учетные данные в Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)