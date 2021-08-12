---
title: Разрешения и согласие API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932110"
---
# <a name="api-permissions-and-consent"></a>Разрешения и согласие API

Приложения, которые интегрируются с платформа удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным. Реализация модели авторизации обновлена на конечной точке платформа удостоверений Майкрософт. Он изменяет взаимодействие приложения с платформа удостоверений Майкрософт. [Разрешения и согласие](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) в конечной точке платформа удостоверений Майкрософт основные понятия этой модели авторизации, включая области, разрешения и согласие.

Платформа [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) упрощает разработку веб-приложений с несколькими клиентами и местных клиентов. Эти приложения позволяют войти в учетные записи пользователей из клиента Azure AD, который отличается от того, где зарегистрировано приложение. Кроме того, им может потребоваться доступ к веб-API Graph API Microsoft (для доступа к Azure AD, Intune и службам в Microsoft 365) и другим API службы Майкрософт, а также к вашим собственным веб-API.

