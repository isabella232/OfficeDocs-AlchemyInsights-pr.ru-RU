---
title: Ошибка при проверке маркера доступа во время выполнения анализа настольных систем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741256"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Ошибка "ошибка при проверке маркера доступа" во время входящей миграции настольных систем

Эта ошибка обычно наблюдается, когда истечет срок действия маркера проверки подлинности. Как правило, обновление страницы обновляет токен. Однако эта проблема может быть недоступна, если к учетной записи, используемой для аналитики на системной плате, применяются какие политики условного доступа. Вы можете просмотреть журналы входа Azure AD на портале Azure, чтобы проверить наличие неудачных попыток входа для учетной записи, используемой для входящей миграции настольных систем.

Для получения дополнительных сведений о условном доступе перейдите [в план развертывания условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).