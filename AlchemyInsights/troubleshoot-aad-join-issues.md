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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403875"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Устранение неполадок в окнах Azure AD

1. Если вы впервые настраивали регистрации устройств, убедитесь, что вы рассмотрели введение в управление устройствами в [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) которое поможет вам получить устройства под управлением в Azure AD. 
1. Если вы непосредственно регистрируете устройства в Azure AD и регистрируете их в Intune, необходимо [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) убедиться, что вы настроили [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) и сначала настроили лицензирование.
1. Убедитесь, что вы уполномочены выполнять операции в Azure AD. Только глобальный администратор в Azure AD может управлять настройками регистрации устройств.
1. Чтобы присоединиться к реализации Azure AD, см. в [статью Plan Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Дополнительные сведения об устранении распространенных проблем с помощью приложения Azure AD см. в faq Azure [Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) и для устройства Windows 10 pro см. в материале [Unable to join Windows 10 Pro machine to Azure AD .](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
