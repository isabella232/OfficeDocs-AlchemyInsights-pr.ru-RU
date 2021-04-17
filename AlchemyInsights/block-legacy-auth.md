---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820191"
---
# <a name="blocking-legacy-authentication"></a>Блокировка устаревшей проверки подлинности

Традиционная аутентификация — это термин, обозначающий запрос на проверку подлинности, который делают:

- Старые клиенты Office, которые не используют современную проверку подлинности (например, клиент Office 2010).

- Любые клиенты, использующие устаревшие почтовые протоколы, например IMAP/SMTP/POP3.

Дополнительные сведения о блокировке устаревшей проверки подлинности и в том, что касается включения современной проверки подлинности, обратитесь к [блокированию устаревшей проверки подлинности.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

По умолчанию безопасность в Azure Active Directory (Azure AD) упрощает безопасность и помогает защитить организацию. По умолчанию в безопасности содержатся преднастройные параметры безопасности для распространенных атак.
Дополнительные сведения о дефолтах безопасности можно найти в этой [ссылке.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**Примечание.** Если клиент был создан 22 октября 2019 г. или после него, возможно, вы столкнулись с новым поведением по умолчанию и уже включили в клиенте по умолчанию безопасность.  Чтобы защитить всех пользователей, для всех созданных новых клиентов в настоящее время выкатываются по умолчанию.
