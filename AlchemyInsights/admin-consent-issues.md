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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888322"
---
# <a name="admin-consent-issues"></a>Проблемы с согласием администратора

1. Разрешить рабочий [процесс согласия администратора,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) чтобы пользователи могли запрашивать утверждение администратора непосредственно с экрана согласия.

1. Если во время получения согласия вы или пользователи приложения видите непредвиденные ошибки, см. эту статью для устранения неполадок: непредвиденное сообщение об ошибке при выполнении согласия [на приложение.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Узнайте больше о согласии администратора на [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) платформе удостоверений [Майкрософт,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)о работе запроса согласия и о том, как оценить запрос согласия администратора на весь [клиент.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Приложения, которые интегрируются с платформой удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным. Реализация модели авторизации была обновлена в конечной точке платформы удостоверений Майкрософт, и она изменяет то, как приложение должно взаимодействовать с платформой удостоверений Майкрософт. Обзор [этой модели](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) авторизации, включая области, разрешения и согласие, см. в сведениях о разрешениях и согласиях в конечной точке платформы удостоверений Майкрософт.