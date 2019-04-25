---
title: Установка Office на сервере терминалов — Нелицензировано
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410135"
---
# <a name="installing-office-on-a-terminal-server"></a>Установка Office на сервере терминалов

Для развертывания Office 365 профессиональный плюс на Windows Server с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:
  
- Вы должны иметь план Office 365, включающий Office 365 профессиональный плюс, например Office 365 Enterprise E3 или Enterprise "\". Планы Office 365 для бизнеса и Office 365 бизнес премиум не включают Office 365 профессиональный плюс.
    
- Необходимо включить активацию на [общем компьютере](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Если вы хотите установить Office 365 профессиональный плюс для RDS на портале Office 365, * *, *где используются параметры установки по умолчанию* * *, выполните указанные ниже действия. 
  
1. Проверьте, какой план Office 365 у вас есть. [Узнайте, как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. При необходимости переключитесь на другой план Office 365. [Узнайте, как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Если Office уже установлен на сервере RDS с помощью других планов Office 365, удалите его. Например, с помощью панели \> управления удалите программу. Удаление с помощью [помощника по поддержке и восстановленИю Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы. 
    
4. На сервере RDS Войдите на портал Office 365 с помощью учетной записи администратора и [установите Office 365 профессиональный плюс](https://portal.office.com/OLS/MySoftware.aspx).
    
5. После установки Office * * *не открывайте и не входите в* приложение Office * *. 
    
6. На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.
    
1. Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду выполнить. В поле Открыть введите regedit **** и нажмите кнопку ОК. 
    
2. Выберите Да, если будет предложено разрешить редактору реестра вносить изменения на устройстве.
    
3. В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе хкэй_локал_мачине\софтваре\микрософт \оффице\кликкторун\конфигуратион. 
    
7. На сервере RDS * * *выполните вход в качестве конечного пользователя* * * и [Убедитесь, что активация на общем компьютере включена для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Для получения дополнительных сведений о предварительных требованиях и инструкциях по настройке для настраиваемых установок с помощью средства развертывания Office, ознакомьтесь со статьей [развертывание office 365 профессиональный плюс с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Устранение ошибок, связанных с активацией на общедоступном компьютере, можно найти в статье [устраненИе неполадок при активации на общем компьютере для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

