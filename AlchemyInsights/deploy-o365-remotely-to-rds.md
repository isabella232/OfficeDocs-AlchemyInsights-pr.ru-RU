---
title: Развертывание Office 365 профессиональный плюс для совместного использования в RDS, сервере терминалов или VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959472"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Развертывание Office 365 профессиональный плюс для совместного использования в RDS, сервере терминалов или VDI

Чтобы развернуть Office 365 профессиональный плюс с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:
- У вас должен быть план Microsoft 365 для бизнеса или план Office 365, включающий Office 365 профессиональный плюс, например Office 365 Enterprise E3 или Enterprise ".
   > [!NOTE] 
   > Планы Office 365 для бизнеса и Office 365 бизнес премиум не включают Office 365 профессиональный плюс.
- Необходимо включить [активацию на общем компьютере](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Вы также можете скачать и запустить [Помощник по поддержке и восстановлению Майкрософт](https://aka.ms/SaRA_OfficeSCA_M365Portal) , чтобы установить Office 365 профессиональный плюс в режиме активации на общем компьютере.

Дополнительные сведения о предварительных требованиях, инструкции по установке и рекомендации по настройке для установки с помощью средства развертывания Office можно найти в статье [deploy office 365 профессиональный плюс с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Устранение ошибок, связанных с активацией на общем компьютере:
- Сведения [об устранении неполадок при активации на общем компьютере для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Ознакомьтесь [со статьей сброс состояния активации Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Если вы хотите установить Office 365 профессиональный плюс в RDS из центра администрирования Майкрософт 365, ***использующего параметры установки по умолчанию***, выполните следующие действия:

1.  Проверьте, какой план Office 365 у вас есть. [Инструкции.](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
2.  При необходимости переключитесь на другой план Office 365. [Инструкции.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
3.  Если Office уже установлен на сервере RDS с помощью других планов Office 365, удалите его. Например, с помощью **панели** > управления**удалите программу**. Удаление с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы.
4.  На сервере RDS Войдите в центр администрирования Microsoft 365 с учетной записью администратора и [установите Office 365 профессиональный плюс](https://portal.office.com/OLS/MySoftware.aspx).
5.  После установки Office ***не открывайте и не входите*** в приложения Office.
6.  На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.
   1. Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду **выполнить**. В поле Открыть введите **regedit**и нажмите кнопку **ОК**.
   2. Выберите **Да** , если будет предложено разрешить редактору реестра вносить изменения на устройстве.
   3. В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе HKEY_LOCAL_MACHINE \софтваре\микрософт \оффице\кликкторун\конфигуратион.
   4. На сервере RDS ***выполните вход в качестве конечного пользователя*** и [Убедитесь, что активация на общем компьютере включена для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

