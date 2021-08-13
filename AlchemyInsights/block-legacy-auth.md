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
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968894"
---
# <a name="blocking-legacy-authentication"></a>Блокировка устаревшей проверки подлинности

Традиционная аутентификация — это термин, обозначающий запрос на проверку подлинности, который делают:

- Более Office клиентов, которые не используют современную проверку подлинности (например, Office 2010).

- Любые клиенты, использующие устаревшие почтовые протоколы, например IMAP/SMTP/POP3.

Дополнительные сведения о блокировке устаревшей проверки подлинности и в том, что касается включения современной проверки подлинности, обратитесь к [блокированию устаревшей проверки подлинности.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

По умолчанию Azure Active Directory (Azure AD) упрощают безопасность и помогают защитить организацию. По умолчанию в безопасности содержатся преднастройные параметры безопасности для распространенных атак.
Дополнительные сведения о дефолтах безопасности можно найти в этой [ссылке.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**Примечание.** Если клиент был создан 22 октября 2019 г. или после него, возможно, вы столкнулись с новым поведением по умолчанию и уже включили в клиенте по умолчанию безопасность.  Чтобы защитить всех пользователей, для всех созданных новых клиентов в настоящее время выкатываются по умолчанию.
