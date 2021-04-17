---
title: Значок календаря не отображается в клиенте Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819966"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Значок календаря не отображается в клиенте Teams

Для вкладки «Календарь» в Teams требуется доступ к почтовому ящику Exchange через веб-службы Exchange. Почтовый ящик Exchange может быть онлайн или локальным. Для пользователей в сети, которые не видят вкладку «Календарь», убедитесь, что они [лицензированы для почтового ящика Exchange Online, и почтовый ящик включен](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Если у пользователя есть действующий почтовый ящик в Exchange Online, но он по-прежнему не видит вкладку «Календарь», возможно, возникла проблема с сетью. Используйте [анализатор удаленного подключения Microsoft](https://testconnectivity.microsoft.com/)и запустите **тесты подключения веб-служб Microsoft Exchange** для затронутого пользователя.

Наконец, проверьте [приложение Teams - политики настройки приложения](https://admin.teams.microsoft.com/policies/app-setup), чтобы убедиться, что приложение «Календарь» не было удалено из политики, применяемой к пользователю (скорее всего, **глобальной (по умолчанию для всей организации)**.

Если ваши пользователи размещены локально, вы должны подтвердить, что ваша гибридная конфигурация исправна. Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок.

Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
