---
title: Устранение неполадок с регистрацией Windows устройств в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981054"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Устранение неполадок с регистрацией Windows устройств в Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему.
  
Некоторые распространенные сообщения об ошибках и действия по разрешению:
  
 **Программное обеспечение не может быть установлено, 0x80cf4017:** Срок действия сертификата учетной записи истек. Повторно скачайте пакет программного обеспечения pc Client в консоли администрирования Intune. Просмотрите эту документацию для получения дополнительных сведений.
  
 **Код ошибки 0x801c0003:** Ошибка может возникать в следующих сценариях:
  
-  У пользователя зарегистрировано больше устройств, чем лимит устройства. Просмотрите эти [документы, чтобы удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить ограничение устройства.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Пользователи могут присоединяться к устройствам в Azure AD" задают "нет". Установите его для всех или выберите пользователей. Просмотрите [эту документацию](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) для получения дополнительных сведений.

-  Устройство уже зарегистрировано другим пользователем. В этом случае удалите устройство из консоли Azure Intune или снимите устройство вручную перед повторной попыткой.

-  Устройство Windows 10 Домашняя. Только Windows 10 Pro, образовательные Enterprise могут присоединиться к Azure Active Directory.

Дополнительные ресурсы для решения проблемы:
  
-  Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации. Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе.

-  Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Узнайте, как зарегистрировать Windows устройства в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
