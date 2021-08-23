---
title: Мое приложение не отображается в управлении приложениями
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362422"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Мое приложение не отображается в управлении приложениями

Если приложение не отображается в управлении приложениями, проверьте следующее:

1. Перейдите [в Azure AD](https://aad.portal.azure.com/) и найдите код приложения для приложения, ища имя приложения в верхней панели на странице Обзор.

1. Доступ Graph Explorer и поиск ID приложения в основной службе с помощью этого запроса и замены соответствующего <appId> ID приложения: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "AppId: <appId> >

1. Если результаты не возвращаются, поиск ID приложения в приложении с помощью этого запроса и замена соответствующего <appId> ID приложения: < https://graph.microsoft.com/v1.0/applications? $search= "AppId: <appId> ">

Если у вас проблемы с запросом, см. в [ссылке Получить поддержку.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Дополнительные сведения и сведения о приложениях в управлении приложениями см. в дополнительных сведениях о видимости [и сведениях.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Дополнительные сведения о просмотре приложений см. в [обзоре приложений.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
