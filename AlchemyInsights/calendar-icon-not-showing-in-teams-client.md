---
title: Значок календаря не отображается в клиенте Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932196"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Значок календаря не отображается в клиенте Teams

Для вкладки «Календарь» в Teams требуется доступ к почтовому ящику Exchange через веб-службы Exchange. Почтовый ящик Exchange может быть онлайн или локальным. Для пользователей в сети, которые не видят вкладку «Календарь», убедитесь, что они [лицензированы для почтового ящика Exchange Online, и почтовый ящик включен](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Если у пользователя есть действующий почтовый ящик в Exchange Online, но он по-прежнему не видит вкладку «Календарь», возможно, возникла проблема с сетью. Используйте [анализатор удаленного подключения Microsoft ](https://testconnectivity.microsoft.com/)и запустите **тесты подключения веб-служб Microsoft Exchange** для затронутого пользователя.

Наконец, проверьте [приложение Teams - политики настройки приложения](https://admin.teams.microsoft.com/policies/app-setup), чтобы убедиться, что приложение «Календарь» не было удалено из политики, применяемой к пользователю (скорее всего, **глобальной (по умолчанию для всей организации)**.

Если ваши пользователи размещены локально, вы должны подтвердить, что ваша гибридная конфигурация исправна. Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок.

Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
