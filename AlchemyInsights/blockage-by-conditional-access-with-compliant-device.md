---
title: Условный доступ блокирует меня при использовании соответствующего устройства
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897983"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Условный доступ блокирует меня при использовании соответствующего устройства

**Настоятельно рекомендуемые инструменты**

- [Средство устранения неполадок с регистрацией устройств](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — комплексное средство, помогающее устранять наиболее распространенные проблемы с регистрацией устройств.
- [Сценарий тестирования подключения регистрации устройств](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — средство, используемое для обеспечения доступа устройства к конечным точкам регистрации устройств в системной учетной записи.
- [Сценарий очистки устройств Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) — средство, используемое для поиска устаревших устройств в среде и управления ими.

Вот некоторые распространенные причины, по которым условный доступ не удается использовать для соответствующих устройств или по которым пользователи получают сообщение **Вы не можете отсюда перейти туда** во время запроса на вход в ресурс организации.

1. **Устройство не соответствует требуемому состоянию в MDM**:

Проверьте, что устройство зарегистрировано в утвержденном поставщике MDM, например в Intune, и *помечено как соответствующее требованиям*. Дополнительные сведения об Intune см. в [этом документе](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Для лучшего понимания соответствия устройств требованиям и Intune см. раздел [Использование политики соответствия, позволяющей установить правила для устройств, управляемых с помощью Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Если у вас возникли проблемы с регистрацией устройства в Intune, сведения об устранении неполадок см. в статье [Устранение неполадок с регистрацией устройств в Майкрософт](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Для дополнительной поддержки по Intune создайте запрос в службу поддержки. Для этого посетите страницу [справки и поддержки по Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Устройство не присоединилось к сети организации**:

Для доступа к ресурсам организации устройство должно быть присоединено к сети организации через прямое подключение или виртуальную частную сеть (VPN), а также присоединено к локальной сети или Azure Active Directory. Чтобы присоединить устройство к сети организации, см. статью [Присоединение рабочего устройства к сети организации](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Чтобы зарегистрировать личное устройство или устройство BYOD, см. статью [Регистрация личного устройства в сети организации](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Чтобы проверить, присоединилось ли устройство к сети, выполните действия для зарегистрированных устройств [здесь](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered), а для рабочих устройств — [здесь](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Чтобы определить, что область проблемы ограничена подключением к сети организации, выполните инструкции ниже.

    1. Войдите в Windows с помощью рабочей или учебной учетной записи, например ivan@contoso.com. 
    2. Подключитесь к сети организации через VPN или DirectAccess.
    3. После подключения нажмите клавишу **Windows+L**, чтобы заблокировать устройство.
    4. Разблокируйте устройство с помощью своей рабочей или учебной учетной записи, а затем попробуйте снова получить доступ к проблемному приложению или службе.

Если вы вновь видите сообщение об ошибке **Вы не можете отсюда перейти туда**, скорее всего, у проблемы другая причина.

3. **Операционная система не поддерживается**:

Используйте поддерживаемую версию операционной системы, в том числе:

- **Клиент Windows**: Windows 7 или более поздние версии

- **Windows Server**: Windows Server 2008 R2 или более поздние версии

- **macOS**: macOS X или более поздние версии

- **Android и iOS**: последняя версия мобильных операционных систем Android и iOS

4. **Веб-браузер не поддерживается**:

Ниже приведены поддерживаемые браузеры. Для поддержки Chrome в Windows версии 1703 или более поздних версиях требуется расширение "Учетные записи Windows 10". Для Microsoft Edge версии 85 и более поздних версий пользователь должен выполнить вход, чтобы правильно передавать сведения о соответствии устройства. Дополнительные сведения см. [здесь](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Дополнительные сведения о сообщении **Вы не можете перейти туда** и инструкции по устранению неполадок см. [здесь](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
