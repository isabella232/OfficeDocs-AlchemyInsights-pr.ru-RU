---
title: Устранение неполадок в окнах Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939932"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Устранение неполадок в окнах Azure AD

1. Если вы впервые настраивали регистрации устройств, убедитесь, [](https://docs.microsoft.com/azure/active-directory/devices/overview) что вы рассмотрели введение в управление устройствами в Azure Active Directory, которое поможет вам получить устройства под управлением в Azure AD. 
1. Если вы непосредственно регистрируете устройства в Azure AD и регистрируете их в Intune, необходимо [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) убедиться, что вы настроили [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) и сначала настроили лицензирование.
1. Убедитесь, что вы уполномочены выполнять операции в Azure AD. Только глобальный администратор Microsoft Azure AD может управлять параметрами регистрации устройств.
1. Чтобы присоединиться к реализации Azure AD, см. в [статью Plan Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Дополнительные сведения об устранении распространенных проблем с помощью присоединиться к Azure AD см. в faq Azure [Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) и для Windows 10 профессиональных устройств см. в материале [Unable to join Windows 10 Pro machine to Azure AD . Необходимо](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) обновить до - Microsoft Community
