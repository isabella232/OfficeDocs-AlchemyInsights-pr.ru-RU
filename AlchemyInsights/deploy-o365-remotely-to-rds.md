---
title: Развертывание Приложения Microsoft 365 для предприятий для общего использования в RDS, Terminal Server или VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041019"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Развертывание Приложения Microsoft 365 для предприятий для общего использования в RDS, Terminal Server или VDI

Чтобы развернуть Приложения Microsoft 365 с помощью служб удаленного рабочего стола (RDS), ранее служб терминалов, необходимо:

- Используйте простое исправление, чтобы включить TLS 1.2 по умолчанию, если вы используете старую версию Windows (например, Windows 7 SP1, Windows Server 2008 R2). Дополнительные сведения см. в дополнительных сведениях об обновлении, чтобы включить [TLS 1.1 и TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)в качестве безопасных протоколов по умолчанию в WinHTTP в Windows . 
- У вас есть план, включавший Приложения Microsoft 365 для предприятий (ранее Office 365 Плюс). Например, Office 365 E3 или Microsoft 365 E5 или любой план, который включает в себя десктопную версию Project или Visio, например Project, план 3 или Visio, план 2, или план Microsoft 365 бизнес премиум, который также включает Приложения Microsoft 365 для бизнеса.
- Включение активации общего компьютера. Дополнительные сведения см. в [обзоре активации](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)общих компьютеров для Приложения Microsoft 365.

**Примечание.** Чтобы установить Приложения Microsoft 365 в режиме активации общего компьютера, скачайте и [запустите microsoft помощник по поддержке и восстановлению](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Дополнительные сведения о необходимых предпосылках, инструкциях по настройке и руководстве по настройке установок с помощью средства развертывания Office см. в Приложения Microsoft 365 Deploy Приложения Microsoft 365 с помощью служб удаленного рабочего [стола.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Чтобы устранить ошибки, связанные с активацией общего компьютера, см. в разделе:

- [Устранение неполадок с активацией общего компьютера для Приложения Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Сброс приложений Microsoft 365 до корпоративного состояния активации.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Если вы хотите установить Приложения Microsoft 365 на RDS из Центр администрирования Microsoft 365, в котором используются параметры установки по умолчанию, выполните следующие действия:

1. Проверьте, Microsoft 365 у вас есть план. Дополнительные сведения см. [в журнале What subscription do I have?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. При необходимости переключение на другой Microsoft 365 плана. Дополнительные сведения см. [в дополнительных сведениях об обновлении к другому плану.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Если Приложения Microsoft 365 уже установлен на сервере RDS с использованием любых других несовместимых планов, отсоединять его, перенастроив панель управления, чтобы удалить   >  **программу.** Если у вас проблемы, удалить, скачав [Microsoft помощник по поддержке и восстановлению](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. На сервере RDS впишитесь в Центр администрирования Microsoft 365 с учетной записью администратора и [установите Office](https://portal.office.com/OLS/MySoftware.aspx).

   После Office не открывайтесь и не впишитесь в Office приложения.

1. На сервере RDS включить активацию общего компьютера путем редактирования реестра:

   1. Щелкните правой кнопкой Windows в левом нижнем углу экрана и выберите **Run**. В поле Открыть введите команду **regedit** и нажмите кнопку **ОК**.

   1. При запросе разрешить редактору реестра вносить изменения на устройство выберите **Да**.

   1. В редакторе реестра в HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration добавьте строковую величину **SharedComputerLicensing** с параметром **1** .

1. На сервере RDS включайся как конечный пользователь и убедитесь, что активация общего компьютера включена для Приложения Microsoft 365. 

   Подробные сведения см. в [материале Verify that shared computer activation is enabled for Приложения Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)