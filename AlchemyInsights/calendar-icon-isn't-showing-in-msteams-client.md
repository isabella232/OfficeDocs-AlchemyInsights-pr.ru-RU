---
title: Значок Calendar не отображается в Microsoft Teams клиенте
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120017"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Значок Calendar не отображается в Microsoft Teams клиенте

**Вкладка** Calendar в Teams требует доступа к почтовому Exchange через Exchange веб-службы. Почтовый Exchange может быть Online или On-Premises. Для пользователей в Интернете, которые не видят вкладку **Calendar,** убедитесь, что они лицензированы для Exchange Online почтового ящика и включен [почтовый ящик](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Если пользователи находятся в локальном помещении, необходимо подтвердить, что гибридная конфигурация здорова. Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок. Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Дополнительные сведения и действия по устранению неполадок см. в Microsoft Teams [и Exchange Server взаимодействия.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
