---
title: Устранение неполадок с регистрацией устройств Android в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709011"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Устранение неполадок с регистрацией устройств Android в Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему.
  
Некоторые распространенные проблемы и действия по разрешению:
  
 **Ошибка устройства, не зашифрованная на портале компании:** Новые версии Android, особенно начиная с v7.0, требуют запуска пароля, чтобы убедиться, что ваше устройство полностью зашифровано. Распространенные решения — включить пин-код запуска или полностью шифровать устройство. Дополнительные [сведения просмотрите](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) в этом документе.
  
 **Устройства не могут провериться в службе Intune** или отображаться как "Нездоровые" в консоли администрирования Intune: Некоторые устройства Samsung 4.4 и 5.5 могут не проверяться в службе. Существует 3 возможных решения этой проблемы:
  
1. Вручную откройте приложение Портал компании Intune, которое автоматически инициирует синхронизацию устройства.

2. Обновление устройства до Android 6.0 или более.

3. Отключение смарт-менеджера Samsung от управления порталом компании Intune. Просмотрите [этот документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для получения дополнительных сведений по этим вопросам и решениям.

 **Тип лицензии пользователя** Недействительный или имя пользователя, не распознаваемая **ошибка:** пользователю необходимо получить лицензию Intune или EMS. Просмотрите эти документы, чтобы назначить лицензию через: Центр администрирования Office или портал Azure.
  
Дополнительные ресурсы для решения проблемы:
  
1. Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации. Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе.

2. Просмотрите [этот документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) для списка распространенных ошибок, которые препятствуют регистрации и разрешений для каждого из них.

3. [Узнайте, как зарегистрироваться на устройствах Android в Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
