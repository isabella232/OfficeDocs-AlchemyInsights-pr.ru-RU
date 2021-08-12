---
title: Произошла ошибка проверки ошибки маркера доступа во время посадки в Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946628"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Ошибка "Ошибка проверки маркера доступа" во время бортовой обработки Desktop Analytics

Эта ошибка обычно наблюдается при истечении срока действия маркера проверки подлинности. Обычно обновление страницы обновляет маркер. Однако эта проблема может сохраняться, если к учетной записи, используемой для настольной аналитики, применяются какие-либо политики условного доступа. Вы можете просмотреть журналы Входа Azure AD на портале Azure, чтобы узнать, есть ли сбои входа для учетной записи, используемой для onboarding Desktop Analytics.

Дополнительные сведения об условном доступе можно получить на сайте [Plan your Conditional Access deployment.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)