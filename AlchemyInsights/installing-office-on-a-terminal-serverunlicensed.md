---
title: Установка office на сервере терминалов - нелицензированный
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486501"
---
# <a name="installing-office-on-a-terminal-server"></a>Установка Office на сервере терминалов

Для развертывания Office 365 профессиональный плюс в Windows Server с помощью служб удаленных рабочих столов (RDS), прежнее название служб терминалов:
  
- Необходимо иметь план Office 365, которая включает в себя Office 365 профессиональный плюс, таких как Office 365 для предприятий E3 или Enterprise E5. Планы Office 365 для бизнеса и Office 365 бизнеса расширенный не включать Office 365 ProPlus.
    
- Необходимо включить [активацию совместно используемый компьютер](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Если вы хотите установить Office 365 ProPlus на служб удаленных рабочих СТОЛОВ с портала Office 365 ** *с использованием параметров установки по умолчанию* **, выполните следующие действия: 
  
1. Проверьте план Office 365, у вас есть. [Узнайте, как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. При необходимости переключитесь различных Office 365. [Узнайте, как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Если Office уже установлен на сервере служб удаленных рабочих СТОЛОВ, с использованием других планов Office 365, ее необходимо удалите. Например, выбрав пункты панель управления \> удаление программы. Удалите с помощью [службы поддержки Майкрософт и помощник по восстановлению](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если вы используете за ошибок. 
    
4. На сервере служб удаленных рабочих СТОЛОВ войдите в портал Office 365 с помощью учетной записи администратора и [установить Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. После установки Office ** *не открывать или входа в* ** в любое приложение Office. 
    
6. На сервере служб удаленных рабочих СТОЛОВ активации совместно используемый компьютер с помощью реестра, выполнив следующие действия:
    
1. Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду выполнить. В поле Открыть введите **команду regedit**и нажмите кнопку «ОК». 
    
2. Нажмите кнопку Да при отображении запроса на разрешение редактор реестра для внесения изменений в устройстве.
    
3. В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в реестр \Office\ClickToRun\Configuration. 
    
7. На сервере служб удаленных рабочих СТОЛОВ ** *Вход как пользователь* ** и [Убедитесь, что активации совместно используемый компьютер включен для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Для получения дополнительных сведений о необходимых компонентов, инструкции по установке и рекомендации по настраиваемой установки с помощью средства развертывания Office можно найти [Развертывание Office 365 профессиональный плюс с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Для устранения ошибок, связанных с активацией совместно используемый компьютер, ознакомьтесь с разделом [Устранение проблем, связанных с активацией совместно используемый компьютер для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

