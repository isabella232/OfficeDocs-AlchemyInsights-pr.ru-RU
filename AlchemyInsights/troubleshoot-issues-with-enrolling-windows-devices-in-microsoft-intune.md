---
title: Устранение неполадок, связанных с регистрацией устройств Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665845"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Устранение неполадок, связанных с регистрацией устройств Windows в Microsoft Intune

Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему.
  
Ниже приведены наиболее распространенные сообщения об ошибках и способы их устранения.
  
 **Не удается установить программное обеспечение, 0x80cf4017:** Срок действия сертификата учетной записи истек. Повторно Скачайте пакет клиентского программного обеспечения ПК в консоли администрирования Intune. Просмотрите эту документацию, чтобы получить дополнительные сведения.
  
 **Код ошибки 0x801c0003:** Ошибка может возникать в следующих сценариях:
  
-  У пользователя больше устройств, зарегистрированных по сравнению с предельным числом устройств. Просмотрите эти документы, чтобы [удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить максимальное количество устройств](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  Для параметра "пользователи могут присоединяться к устройствам в Azure AD" задано значение "нет". Задайте для него значение все или выберите Пользователи. Просмотрите [эту документацию](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , чтобы получить дополнительные сведения.

-  Устройство уже зарегистрировано другим пользователем. В этом случае удалите устройство из консоли Azure Intune или вручную отрегистрируйте устройство, прежде чем повторять попытку.

-  Устройство является Windows 10 Домашняя. Присоединиться к Azure Active Directory могут только Windows 10 профессиональная, учебные и корпоративные SKU.

Дополнительные материалы по решению возникшей проблемы:
  
-  Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации. Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения.

-  Просмотрите эти документы, чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать проблемы с документацией: [руководство по устранению неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Устранение неполадок документа](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Узнайте, как зарегистрировать устройства Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
