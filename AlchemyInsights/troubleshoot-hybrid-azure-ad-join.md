---
title: Устранение неполадок с гибридным присоединением к Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939284"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Устранение неполадок с гибридным присоединением к Azure AD

Настоятельно рекомендуется обеспечить доступ устройства к конечным точкам регистрации устройств в системной учетной записи с помощью [сценария тестирования подключения регистрации устройств](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Если вы впервые настраиваете регистрацию устройства, ознакомьтесь с [Введением в управление устройствами в Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), чтобы узнать, как установить контроль Microsoft Azure AD над устройством.
1. Если вы регистрируете устройство непосредственно в Microsoft Azure AD, а затем в Intune, сначала [настройте Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и убедитесь в наличии [лицензий](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Убедитесь, что у вас есть права на выполнение операций в Microsoft Azure AD и локальной службе Active Directory. Только глобальный администратор Microsoft Azure AD может управлять параметрами регистрации устройств. Кроме того, для настройки автоматической регистрации в локальной службе Active Directory необходимы права администратора Active Directory и AD FS (если применимо).

Дополнительные сведения об устранении возможных проблем с гибридным присоединением см. в статье [Устранение неполадок с гибридным присоединением](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Сведения о настройке гибридного присоединения к Azure AD и управлении устройствами с использованием портала Microsoft Azure AD см. в статьях [Настройка устройств с гибридным присоединением к Azure AD (присоединенных к локальному домену)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) и [Управление устройствами с использованием портала Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Чтобы устранить распространенные проблемы с гибридным присоединением к Azure Active Directory (AD), см. раздел [Часто задаваемые вопросы о гибридном присоединении к Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
