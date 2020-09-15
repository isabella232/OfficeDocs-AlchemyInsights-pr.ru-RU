---
title: Устранение неполадок, связанных с регистрацией устройств Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658891"
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

-  Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Узнайте, как зарегистрировать устройства Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
