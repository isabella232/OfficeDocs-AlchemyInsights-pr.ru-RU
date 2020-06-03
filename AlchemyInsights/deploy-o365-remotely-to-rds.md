---
title: Развертывание приложений Microsoft 365 для предприятий для совместного использования в RDS, сервере терминалов или VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507599"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Развертывание приложений Microsoft 365 для предприятий для совместного использования в RDS, сервере терминалов или VDI

Чтобы развернуть приложения Microsoft 365 для предприятия с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:
- Необходим план Microsoft 365 для бизнеса или план Office 365, включающий приложения Microsoft 365 для предприятия, такие как Office 365 Enterprise E3 или Enterprise "\".
   > [!NOTE] 
   > Стандартные планы приложений Microsoft 365 для бизнеса и Microsoft 365 бизнес премиум не включают приложения Microsoft 365 для предприятия.
- Необходимо включить [активацию на общем компьютере](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Вы также можете скачать и запустить [Помощник по поддержке и восстановлению Майкрософт](https://aka.ms/SaRA_OfficeSCA_M365Portal) для установки приложений Microsoft 365 для предприятий в режиме активации на общем компьютере.

Дополнительные сведения о предварительных требованиях, инструкции по установке и рекомендации по настройке для установки с помощью средства развертывания Office можно найти в статье [развертывание приложений Microsoft 365 для предприятий с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Устранение ошибок, связанных с активацией на общем компьютере:
- Сведения об [устранении неполадок при активации на общем компьютере для приложений Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- См. статью [Сброс приложений Microsoft 365 до корпоративного состояния активации](https://go.microsoft.com/fwlink/?linkid=2109218).

Если вы хотите установить приложения Microsoft 365 для Enterprise в RDS из центра администрирования Майкрософт 365, ***использующего параметры установки по умолчанию***, выполните указанные ниже действия.

1.    Проверьте, какая подписка у вас есть. [Инструкции.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2.    При необходимости переключитесь на другую подписку. [Инструкции.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3.    Если Office уже установлен на сервере RDS с помощью любой другой подписки Майкрософт, удалите его. Например, с помощью **панели управления**  >  **удалите программу**. Удаление с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы.
4.    На сервере RDS Войдите в центр администрирования Microsoft 365 с учетной записью администратора и [установите приложения Microsoft 365 для предприятия](https://portal.office.com/OLS/MySoftware.aspx).
5.    После установки Office ***не открывайте и не входите*** в приложения Office.
6.    На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.
   1. Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду **выполнить**. В поле Открыть введите **regedit**и нажмите кнопку **ОК**.
   2. Выберите **Да** , если будет предложено разрешить редактору реестра вносить изменения на устройстве.
   3. В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе HKEY_LOCAL_MACHINE \софтваре\микрософт \оффице\кликкторун\конфигуратион.
   4. ***Выполните вход в качестве конечного пользователя*** на сервере RDS и [Убедитесь, что активация на общем компьютере включена для приложений Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

