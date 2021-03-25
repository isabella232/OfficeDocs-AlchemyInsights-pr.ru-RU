---
title: Развертывание приложений Microsoft 365 для предприятия для общего использования в RDS, Terminal Server или VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200686"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Развертывание приложений Microsoft 365 для предприятия для общего использования в RDS, Terminal Server или VDI

Развертывание приложений Microsoft 365 для предприятия с использованием служб удаленного рабочего стола (RDS), ранее именуемой службами терминалов:

- Необходимо иметь план Microsoft 365 для бизнеса или план Office 365, который включает приложения Microsoft 365 для предприятия, такие как Office 365 Enterprise E3 или Enterprise E5.
   > [!NOTE]
   > Планы Microsoft 365 Apps для бизнеса и Microsoft 365 Business Standard не включают приложения Microsoft 365 для предприятия.
- Необходимо включить [активацию общего компьютера.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Вы также можете скачать и запустить [помощник по поддержке и](https://aka.ms/SaRA_OfficeSCA_M365Portal) восстановлению Майкрософт для установки приложений Microsoft 365 для предприятия в режиме активации общего компьютера.

Дополнительные сведения о необходимых предпосылках, инструкциях по установке и руководстве по настраиваемым установкам с помощью средства развертывания Office см. в рублях [Deploy Microsoft 365 Apps для](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)предприятия с помощью служб удаленного рабочего стола.

Устранение ошибок, связанных с активацией общего компьютера:

- См. [раздел Устранение неполадок с активацией общих компьютеров для Microsoft 365 Apps для предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- См. статью [Сброс приложений Microsoft 365 до корпоративного состояния активации](https://go.microsoft.com/fwlink/?linkid=2109218).

Если вы хотите установить Microsoft 365 Apps для предприятия на RDS из центра администрирования Microsoft 365, который использует параметры установки по умолчанию, используйте следующие действия:

1. Проверьте, какая у вас подписка. [Инструкции.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. При необходимости переключение на другую подписку. [Инструкции.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Если Office уже установлен на сервере RDS с помощью любых других подписок Майкрософт, удалить его. Например, при помощи панели **управления** удалить программу  >  . Если у вас проблемы, удалить с помощью [помощника по](https://aka.ms/SARA-OfficeUninstall-Alchemy) поддержке и восстановлению Майкрософт.
4. На сервере RDS впишитесь в центр администрирования Microsoft 365 с учетной записью администратора и установите [приложения Microsoft 365 для предприятия.](https://portal.office.com/OLS/MySoftware.aspx)
5. После установки Office не открывайтесь и не ***впишитесь в*** приложения Office.
6. На сервере RDS включить активацию общего компьютера, редактировать реестр, следуя следующим шагам:
   1. Щелкните правой кнопкой Windows в нижнем левом углу экрана и выберите **Run**. В поле Открыть введите команду **regedit** и нажмите кнопку **ОК**.
   2. Выберите **Да** при запросе разрешить редактору реестра вносить изменения на устройство.
   3. В редакторе реестра добавьте строковую величину **SharedComputerLicensing** с параметром 1 в соответствии с HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На сервере RDS  включайся как конечный пользователь и убедитесь, что активация общего компьютера включена для Microsoft [365 Apps для предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
