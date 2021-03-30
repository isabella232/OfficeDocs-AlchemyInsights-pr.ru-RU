---
title: Приложение проверки подлинности
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
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403838"
---
# <a name="authentication-app"></a>Приложение проверки подлинности

Если вы глобальный администратор, вы можете быстро узнать о том, что произошло или диагностировать проблемы, связанные с входом пользователя, с помощью диагностики [входов.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Начните диагностику, нажав кнопку["Запуск](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)диагностики". 
1. Найдите событие для анализа, введите сведения о пользователе, приложении, времени входа, id запроса или корреляции.
1. Ознакомьтесь с результатами диагностики, отображающими подробные сведения о том, что произошло и какие действия нужно предпринять, чтобы внести изменения.

**Проверьте применимый сценарий:**

1. Если пользователь не получает push-уведомления в приложении Microsoft Authenticator, убедитесь, что они не показаны под заблокированными пользователями MFA, как описано в Block и [разблокировать пользователей](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Если пользователь не заблокирован для MFA, но не получает push-уведомления, он может открыть приложение Microsoft Authenticator, которое будет тянуть ожидающих запросов на утверждение.
1. В качестве альтернативного метода регистрации пользователь также может щелкнуть кнопку Войти другим способом и выбрать код проверки из мобильного приложения.
1. Приложение Microsoft Authenticator — единственный доступный метод для многих пользователей. [Дополнительные новости о по умолчанию безопасности,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [проверка](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) часто задаваемой вопросы и их устранение.
 
**Рекомендуемые видео**

[Настройка приложения authenticator на новом телефоне (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
