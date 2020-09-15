---
title: Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669261"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune

Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему. 
  
Ниже приведены наиболее распространенные сообщения об ошибках и способы их устранения.
  
- **Достигнута заглушка устройства** У пользователя больше устройств, зарегистрированных по сравнению с предельным числом устройств. Просмотрите эти документы, чтобы [удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить максимальное количество устройств](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Эта служба не поддерживается. Политика регистрации отсутствует:** необходимо настроить или обновить службу push-уведомлений Apple (APNs). Изучите [этот документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , чтобы узнать, как это сделать. 
    
- **Недопустимый тип лицензии пользователя, или имя пользователя не распознано:** Пользователю необходимо назначить лицензию на Intune или EMS. Просмотрите эти документы, чтобы назначить лицензию: [центр администрирования Office](https://docs.microsoft.com/intune/licenses-assign) или [портал Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Дополнительные материалы по решению возникшей проблемы:
  
1. Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации. Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения. 
    
2. Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Узнайте, как зарегистрировать устройства с iOS в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

