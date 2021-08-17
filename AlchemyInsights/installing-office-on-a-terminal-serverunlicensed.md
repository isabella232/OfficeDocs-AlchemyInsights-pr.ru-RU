---
title: Установка офиса на сервер терминала — без лицензии
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055171"
---
# <a name="installing-office-on-a-terminal-server"></a>Установка Office на сервер терминала

Для развертывания Приложения Microsoft 365 для предприятий на сервере Windows с помощью служб удаленного рабочего стола (RDS), ранее именуемой службами терминалов:
  
- Вы должны иметь подписку Microsoft 365, которая включает Приложения Microsoft 365 для предприятий, например Office 365 корпоративный E3 или Enterprise E5. В Приложения Microsoft 365 для бизнеса и Приложения Microsoft 365 для бизнеса Premium не включены Приложения Microsoft 365 для предприятий.

- Необходимо включить активацию [общего компьютера.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Если вы хотите установить Приложения Microsoft 365 для предприятий на RDS из ***Центр администрирования Microsoft 365,*** в котором используются параметры установки по умолчанию, используйте следующие действия.

> [!TIP]
> Вы также можете скачать и запустить [microsoft помощник по поддержке и восстановлению](https://aka.ms/SaRA_OfficeSCA_M365Portal) для установки Приложения Microsoft 365 для предприятий в режиме активации общего компьютера.
  
1. Проверьте, Microsoft 365 подписка у вас есть. [Инструкции](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. При необходимости переключение на другую Microsoft 365 подписку. [Инструкции](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Если Office уже установлена на сервере RDS с помощью любых других Microsoft 365, удалить его. Например, при помощи диспетчерской панели \> удалить программу. Удалить с помощью [Microsoft помощник по поддержке и восстановлению,](https://aka.ms/SARA-OfficeUninstall-Alchemy) если у вас проблемы.

4. На сервере RDS вопишитесь в Центр администрирования Microsoft 365 с учетной записью администратора и [установите Приложения Microsoft 365 для предприятий](https://portal.office.com/OLS/MySoftware.aspx).

5. После Office не открывайтесь и не впишитесь в Office приложения. 

6. На сервере RDS включить активацию общего компьютера, редактировать реестр, следуя следующим шагам:

1. Щелкните правой кнопкой Windows в левом нижнем углу экрана и выберите Run. В поле Открыть введите **regedit** и выберите ОК.

2. Выберите Да при запросе разрешить редактору реестра вносить изменения на устройство.

3. В редакторе реестра добавьте строковую величину **SharedComputerLicensing** с параметром 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На сервере RDS  включайся как конечный пользователь и убедитесь, что активация общего компьютера включена для [Приложения Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Дополнительные сведения о необходимых предпосылках, инструкциях по настройке и руководстве по настраиваемым установкам с помощью средства развертывания Office см. в Приложения Microsoft 365 для предприятий Deploy Приложения Microsoft 365 для предприятий с помощью служб удаленного рабочего [стола.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Чтобы устранить ошибки, связанные с активацией общего компьютера, см. в раздел [Устранение](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)неполадок с активацией общего компьютера для Приложения Microsoft 365 для предприятий .
  