---
title: Устранение неполадок с Регистрация устройств Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486499"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Устранение неполадок с Регистрация устройств Windows Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему сейчас. 
  
Некоторые распространенные сообщения об ошибках и инструкции по устранению неполадок:
  
 **Не удается установить программное обеспечение, 0x80cf4017:** Истек срок действия сертификата учетной записи. Загрузите пакет программного обеспечения клиентском Компьютере в консоли администрирования Intune. Дополнительные сведения о документации. 
  
 **Код ошибки 0x801c0003:** Ошибка может возникнуть в следующих сценариях: 
  
1. У пользователя есть несколько устройств, участвуют превышает ограничение устройства. Просмотрите эти документы, чтобы [Удалить устройство](https://docs.microsoft.com/en-us/intune/devices-wipe) или [Изменение ограничения устройства](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. «Пользователи могут участвовать в устройствах для Azure AD» имеет значение «none». Задайте для него значение all, или выберите пользователей. Ознакомьтесь с [этой документации](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) для получения дополнительных сведений. 
    
3. Устройство уже участвуют другим пользователем. Если это так, удалите его из консоли Azure Intune или вручную unenroll устройства перед повторением.
    
4. Устройство является 10 Windows Home. Только Windows 10 Pro, обучения и Enterprise могут присоединиться к Azure Active Directory.
    
Дополнительные ресурсы, которые помогут устранить проблему:
  
1. [Устранение неполадок в портал Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) используйте для диагностики и устранения распространенных ошибок регистрации. Просмотрите [Этот документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) для получения дополнительных сведений. 
    
2. Просмотрите эти документы, список распространенные ошибки, которые препятствуют регистрации и решения в каждое: [руководство по Устранение неполадок](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Устранение неполадок doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Узнайте, как возможность зачисления устройств Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

