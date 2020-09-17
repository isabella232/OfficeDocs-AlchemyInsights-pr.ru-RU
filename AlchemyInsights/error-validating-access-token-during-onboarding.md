---
title: Ошибка при проверке маркера доступа во время выполнения анализа настольных систем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783564"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Ошибка "ошибка при проверке маркера доступа" во время входящей миграции настольных систем

Эта ошибка обычно наблюдается, когда истечет срок действия маркера проверки подлинности. Как правило, обновление страницы обновляет токен. Однако эта проблема может быть недоступна, если к учетной записи, используемой для аналитики на системной плате, применяются какие политики условного доступа. Вы можете просмотреть журналы входа Azure AD на портале Azure, чтобы проверить наличие неудачных попыток входа для учетной записи, используемой для входящей миграции настольных систем.

Для получения дополнительных сведений о условном доступе перейдите [в план развертывания условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).