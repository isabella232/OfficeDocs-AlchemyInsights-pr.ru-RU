---
title: Устранение неполадок с регистрация Android устройств в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939361"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Устранение неполадок с регистрация Android устройств в Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему сейчас.
  
Некоторые распространенные проблемы и инструкции по устранению неполадок:
  
 **Устройство не зашифрованы ошибка в портал компания:** Новая версия Android, начиная с v7.0, особенно требовать секретный код загрузки для убедитесь в том, что полностью шифруются устройства. Типичные решения, чтобы включить ПИН-код запуска или полностью шифрование устройства. Просмотрите [Этот документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) для получения дополнительных сведений. 
  
 **Устройств не удается проверить с помощью службы Intune или в виде «Неработоспособная» в консоли администрирования Intune:** Некоторые 4.4 Samsung и 5.5 устройств могут не проверять в службу. Существует 3 возможные решения для устранения этой проблемы. 
  
1. Вручную откройте приложение портала компании Intune автоматически начнет синхронизации устройства.
    
2. Обновление устройства Android 6.0 или более поздней версии.
    
3. Отключение смарт-диспетчер Samsung от управления портала компании Intune. Просмотрите [Этот документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для получения подробных сведений о эти проблемы и решения. 
    
 **Недопустимый тип лицензии пользователя** или **имя пользователя не распознается ошибки:** пользователь должен быть назначен Intune или Командной лицензии. Просмотрите эти документы назначение лицензии через: центр администрирования Office или Azure портала. 
  
Дополнительные ресурсы, которые помогут устранить проблему:
  
1. [Устранение неполадок в портал Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) используйте для диагностики и устранения распространенных ошибок регистрации. Просмотрите [Этот документ](https://docs.microsoft.com/intune/help-desk-operators) для получения дополнительных сведений. 
    
2. Просмотрите [Этот документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) содержит список распространенные ошибки, которые препятствуют регистрации и решения для каждого. 
    
3. [Узнайте, как зарегистрировать Android устройств в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

