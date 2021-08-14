---
title: Проблемы с согласием администратора
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952586"
---
# <a name="admin-consent-issues"></a>Проблемы с согласием администратора

1. Включить рабочий [процесс согласия администратора,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) чтобы пользователи могли запрашивать утверждение администратора непосредственно с экрана согласия.

1. Если во время процесса согласия у вас или пользователей приложения возникли непредвиденные ошибки, см. в этой статье действия по устранению неполадок: неожиданная ошибка при выполнении согласия на [приложение.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Узнайте больше [о](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)согласии администратора на [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) платформа удостоверений Майкрософт, о том, как работает запрос на согласие и как оценить запрос на согласие администратора для всего [клиента.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Приложения, которые интегрируются с платформа удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным. Реализация модели авторизации была обновлена на конечной точке платформа удостоверений Майкрософт, и она меняет, как приложение должно взаимодействовать с платформа удостоверений Майкрософт. Сведения об этой модели авторизации, включая области, разрешения и [согласие, см.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) в платформа удостоверений Майкрософт в конечной точке.