---
title: Возвращение устройства
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320099"
---
# <a name="device-writeback"></a>Возвращение устройства

Возвращение устройства используется в следующих сценариях:

- Включить [Windows Hello для бизнеса с помощью гибридного развертывания доверия сертификата](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Включить условный доступ на основе устройств к защищенным приложениям ADFS (2012 R2 или выше) (доверчивые доверяющие стороны)

    **Примечание.** Подписка на Azure AD Premium требуется для списания устройств.

Это обеспечивает дополнительную безопасность и уверенность в том, что доступ к приложениям предоставляется только доверенным устройствам. Дополнительные сведения об условном [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) доступе см. в рублях Управление рисками с помощью условного доступа и настройка локального условного доступа с Azure Active Directory [регистрации устройств.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Дополнительные сведения о включаемой записи устройств для устройств см. в [статью Включение записи устройств.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
