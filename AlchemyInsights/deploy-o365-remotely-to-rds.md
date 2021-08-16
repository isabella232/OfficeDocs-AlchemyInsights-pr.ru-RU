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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031491"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Развертывание Приложения Microsoft 365 для предприятий для общего использования в RDS, Terminal Server или VDI

Развертывание Приложения Microsoft 365 для предприятий с помощью служб удаленного рабочего стола (RDS), ранее именуемой службами терминалов:

- Вы должны иметь Microsoft 365 для бизнеса или Office 365, который включает Приложения Microsoft 365 для предприятий, например Office 365 корпоративный E3 или Enterprise E5.
   > [!NOTE]
   > В Приложения Microsoft 365 для бизнеса и Microsoft 365 бизнес стандарт не включены Приложения Microsoft 365 для предприятий.
- Необходимо включить [активацию общего компьютера.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Вы также можете скачать и запустить [microsoft помощник по поддержке и восстановлению](https://aka.ms/SaRA_OfficeSCA_M365Portal) для установки Приложения Microsoft 365 для предприятий в режиме активации общего компьютера.

Дополнительные сведения о необходимых предпосылках, инструкциях по настройке и руководстве по настраиваемым установкам с помощью средства развертывания Office см. в Приложения Microsoft 365 для предприятий Deploy Приложения Microsoft 365 для предприятий с помощью служб удаленного [рабочего стола.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Устранение ошибок, связанных с активацией общего компьютера:

- См. [раздел Устранение неполадок с активацией](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)общего компьютера для Приложения Microsoft 365 для предприятий.
- См. статью [Сброс приложений Microsoft 365 до корпоративного состояния активации](https://go.microsoft.com/fwlink/?linkid=2109218).

Если вы хотите установить Приложения Microsoft 365 для предприятий на RDS из ***Центр администрирования Microsoft 365,*** в котором используются параметры установки по умолчанию, используйте следующие действия:

1. Проверьте, какая у вас подписка. [Инструкции.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. При необходимости переключение на другую подписку. [Инструкции.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Если Office уже установлен на сервере RDS с помощью любых других подписок Майкрософт, его удалить. Например, при помощи панели **управления** удалить программу  >  . Удалить с помощью [Microsoft помощник по поддержке и восстановлению,](https://aka.ms/SARA-OfficeUninstall-Alchemy) если у вас проблемы.
4. На сервере RDS вопишитесь в Центр администрирования Microsoft 365 с учетной записью администратора и [установите Приложения Microsoft 365 для предприятий](https://portal.office.com/OLS/MySoftware.aspx).
5. После Office не открывайтесь и не впишитесь в Office приложения. 
6. На сервере RDS включить активацию общего компьютера, редактировать реестр, следуя следующим шагам:
   1. Щелкните правой кнопкой Windows в нижнем левом углу экрана и выберите **Run**. В поле Открыть введите команду **regedit** и нажмите кнопку **ОК**.
   2. Выберите **Да** при запросе разрешить редактору реестра вносить изменения на устройство.
   3. В редакторе реестра добавьте строковую величину **SharedComputerLicensing** с параметром 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На сервере RDS  включайся как конечный пользователь и убедитесь, что активация общего компьютера включена для [Приложения Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
