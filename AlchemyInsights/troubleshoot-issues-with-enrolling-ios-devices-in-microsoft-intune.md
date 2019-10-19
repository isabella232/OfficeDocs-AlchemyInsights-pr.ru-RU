---
title: Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507016"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune

Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему. 
  
Ниже приведены наиболее распространенные сообщения об ошибках и способы их устранения.
  
- **Достигнута заглушка устройства** У пользователя больше устройств, зарегистрированных по сравнению с предельным числом устройств. Просмотрите эти документы, чтобы [удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить максимальное количество устройств](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Эта служба не поддерживается. Политика регистрации отсутствует:** необходимо настроить или обновить службу push-уведомлений Apple (APNs). Изучите [этот документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , чтобы узнать, как это сделать. 
    
- **Недопустимый тип лицензии пользователя, или имя пользователя не распознано:** Пользователю необходимо назначить лицензию на Intune или EMS. Просмотрите эти документы, чтобы назначить лицензию: [центр администрирования Office](https://docs.microsoft.com/intune/licenses-assign) или [портал Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Дополнительные материалы по решению возникшей проблемы:
  
1. Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации. Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения. 
    
2. Просмотрите эти документы, чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать проблемы с документацией: [руководство по устранению неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [Устранение неполадок документа](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Узнайте, как зарегистрировать устройства с iOS в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

