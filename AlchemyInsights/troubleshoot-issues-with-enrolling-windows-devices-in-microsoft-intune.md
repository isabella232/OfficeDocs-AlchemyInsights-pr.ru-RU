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
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661571"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Устранение неполадок с Регистрация устройств Windows Microsoft Intune

Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему сейчас. 
  
Некоторые распространенные сообщения об ошибках и инструкции по устранению неполадок:
  
 **Не удается установить программное обеспечение, 0x80cf4017:** Истек срок действия сертификата учетной записи. Загрузите пакет программного обеспечения клиентском Компьютере в консоли администрирования Intune. Дополнительные сведения о документации. 
  
 **Код ошибки 0x801c0003:** Ошибка может возникнуть в следующих сценариях: 
  
1. У пользователя есть несколько устройств, участвуют превышает ограничение устройства. Просмотрите эти документы, чтобы [Удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [Изменение ограничения устройства](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. «Пользователи могут участвовать в устройствах для Azure AD» имеет значение «none». Задайте для него значение all, или выберите пользователей. Ознакомьтесь с [этой документации](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) для получения дополнительных сведений. 
    
3. Устройство уже участвуют другим пользователем. Если это так, удалите его из консоли Azure Intune или вручную unenroll устройства перед повторением.
    
4. Устройство является 10 Windows Home. Только Windows 10 Pro, обучения и Enterprise могут присоединиться к Azure Active Directory.
    
Дополнительные ресурсы, которые помогут устранить проблему:
  
1. [Устранение неполадок в портал Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) используйте для диагностики и устранения распространенных ошибок регистрации. Просмотрите [Этот документ](https://docs.microsoft.com/intune/help-desk-operators) для получения дополнительных сведений. 
    
2. Просмотрите эти документы, список распространенные ошибки, которые препятствуют регистрации и решения в каждое: [руководство по Устранение неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Устранение неполадок doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Узнайте, как возможность зачисления устройств Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

