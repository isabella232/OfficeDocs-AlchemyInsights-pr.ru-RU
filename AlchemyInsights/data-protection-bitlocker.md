---
title: DataProtection — bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118607"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Включение шифрования Bitlocker с помощью Intune

Intune Endpoint Protection политики можно использовать для настройки параметров шифрования Bitlocker для Windows устройств. Дополнительные сведения см. Windows 10 (и более поздних) параметров для защиты устройств [с помощью Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Помимо политики Endpoint Protection существует также отчет о шифровании, который предоставляет более подробное представление состояния шифрования для устройств. Этот отчет можно получить на портале MEM в статье **Devices > Monitor,** а затем в **отчете Configuration** select [Encryption](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Если вы найдете, что Bitlocker не включен, как ожидалось, или что профиль, используемый для включения Bitlocker, находится в состоянии ошибки, просмотрите отчет о шифровании, чтобы лучше понять, почему происходит поведение.

Сведения о том, как интерпретировать отчет, включая различные значения состояния шифрования, см. в материале [Monitor device encryption with Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Следует помнить, что многие новые устройства с Windows 10 поддерживают автоматическое шифрование Bitlocker, которое запускается без применения политики MDM. Это может повлиять на применение политики, если параметры по умолчанию настроены. Дополнительные вопросы см. в следующем faq.

Сведения о устранении неполадок с битлокером см. в [Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Вопросы и ответы**

В. Какие выпуски Windows поддерживают шифрование устройств с Endpoint Protection политики?<br>
О. Параметры политики Intune Endpoint Protection реализованы с помощью [CSP Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Не все выпуски или сборки Windows поддерживают CSP Bitlocker. <br><br>

В. Как можно включить Bitlocker на устройствах без необходимости взаимодействия с конечным пользователем?<br>
О. До тех пор, пока будут выполнены необходимые предварительные требования, можно включить bitlocker "Silent Encryption" через Intune. Сведения о требованиях к устройству и параметры политики для обеспечения бесшумного шифрования см. в следующем doc: [Silently Enable Bitlocker Encryption.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

В. Если устройство уже зашифровано с помощью Bitlocker с помощью параметров по умолчанию ОС для метода шифрования и прочности шифра (XTS-AES-128), будет ли применяться политика с различными настройками, автоматически запуская повторное шифрование диска с новыми настройками?<br>
О: Нет. Чтобы применить новые параметры шифра, сначала необходимо расшифровать диск.<br><br>
**Примечание:** Для устройств, зарегистрированных с автопилотом, автоматическое шифрование, которое будет происходить во время OOBE, не запускается до оценки политики Intune, что позволяет использовать параметры, основанные на политике, на месте по умолчанию ОС.
 
В. Если устройство зашифровано в результате применения политики Intune, будет ли оно расшифровываться при удалении этой политики?<br>
О. Удаление политики, связанной с шифрованием, не приводит к расшифровке настроенных дисков.
 
В. Почему политика соответствия требованиям Intune показывает, что на моем устройстве не включен Bitlocker, несмотря на то, что оно включено?<br>
A. Параметр "Bitlocker включен" в политике соответствия требованиям intune использует клиент Windows для проверки состояния здоровья устройств (DHA). Этот клиент измеряет состояние устройства только во время загрузки. Поэтому, если устройство не было перезагружается после завершения шифрования Bitlocker, клиентская служба DHA не будет сообщать о том, что Bitlocker активен.
 
 