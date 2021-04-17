---
title: Устранение неполадок с регистрацией устройств iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823476"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Устранение неполадок с регистрацией устройств iOS в Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему. 
  
Некоторые распространенные сообщения об ошибках и действия по разрешению:
  
- **Достигаемая крышка устройства** У пользователя зарегистрировано больше устройств, чем лимит устройства. Просмотрите эти [документы, чтобы удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить ограничение устройства.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Эта служба не поддерживается. Нет политики регистрации:** служба push-уведомлений Apple (APNS) должна быть настроена или обновлена. Просмотрите [этот документ,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) чтобы узнать, как это сделать. 
    
- **Тип лицензии пользователя недействительный или имя пользователя не распознается:** Пользователю должна быть назначена лицензия Intune или EMS. Просмотрите эти документы, чтобы назначить лицензию через: [Центр администрирования Office или](https://docs.microsoft.com/intune/licenses-assign) портал [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Дополнительные ресурсы для решения проблемы:
  
1. Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации. Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе. 
    
2. Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Узнайте, как зарегистрироваться на устройствах iOS в Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

