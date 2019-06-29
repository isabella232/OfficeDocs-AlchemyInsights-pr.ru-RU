---
title: Устранение неполадок, связанных с регистрацией устройств с Android в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367302"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Устранение неполадок, связанных с регистрацией устройств с Android в Microsoft Intune

Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему.
  
Некоторые распространенные проблемы и способы их устранения.
  
 **Ошибка "устройство не зашифровано" в портале компании:** Более новые версии Android, особенно начиная с версии 7.0, требуют запуска загрузочного кода, чтобы убедиться, что устройство полностью зашифровано. Общие решения позволяют включить ПИН-код запуска или полностью зашифровать устройство. Просмотрите [этот документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , чтобы получить дополнительные сведения.
  
 **Устройства не могут вернуть службу Intune или отобразить как "неработоспособное" в консоли администрирования Intune:** Некоторые устройства Samsung 4,4 и 5,5 могут не вернуть службу. Существует три возможных решения этой проблемы:
  
1. Вручную откройте приложение "Корпоративный портал Intune", которое будет автоматически инициировать синхронизацию устройств.

2. Обновите устройство до Android 6,0 или более поздней версии.

3. Отключение интеллектуального менеджера Samsung от управления порталом компании Intune. Ознакомьтесь с [этим документом](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , чтобы получить дополнительные сведения об этих проблемах и их разрешениях.

 **Недопустимый тип лицензии пользователя** , или **имя пользователя не опознано ошибка:** пользователю должна быть назначена лицензия Intune или EMS. Просмотрите эти документы, чтобы назначить лицензию: центр администрирования Office или портал Azure.
  
Дополнительные материалы по решению возникшей проблемы:
  
1. Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации. Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения.

2. Просмотрите [этот документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать их.

3. [Узнайте, как зарегистрировать устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
