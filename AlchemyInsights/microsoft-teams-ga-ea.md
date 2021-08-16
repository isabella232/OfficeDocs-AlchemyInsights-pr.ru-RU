---
title: Microsoft Teams - Гостевой доступ
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012321"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - Гостевой доступ

Если вам нужна помощь в общении с пользователями за пределами организации в Teams, необходимо решить, следует ли использовать гостевой доступ или внешний доступ [(федерация),](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)или вы можете использовать оба.

Обязательно [просмотрите различия, чтобы](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) понять возможности, доступные для каждого из них.  Например, внешний доступ (федерация) позволяет использовать 1:1 связи, такие как Chat и Presence.  Однако федерационные пользователи не могут Teams совместной работы.  Если вы хотите, чтобы внешний пользователь присоединился к Teams или share Files, необходимо включить гостевой доступ.

**Вариант 1. Включив гостевой доступ** В центре Teams администратора перейдите в [Центр](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) Параметры > для гостей и включив "Разрешить гостевой доступ в Teams".  Для клиента со всеми другими настройками по умолчанию это должно быть все, что вам нужно сделать.  Чтобы настроить конфигурацию гостевого доступа, выполните все действия в списке [гостевого доступа.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) После полной работы необходимо подождать до [24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) часов, чтобы параметры вступили в силу.

Если вы уверены, что выполнили все действия в списке, и это было более 24 часов, попробуйте добавить гостя в [свою команду](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Дополнительные сведения, в том числе видео, см. в гостевом доступе [в Microsoft Teams.](https://docs.microsoft.com/microsoftteams/guest-access)

**Вариант 2. Включи внешний доступ (федерация)** Если вы также хотите включить внешний доступ (Федерация), в центре администрирования Teams перейдите в Центр администрирования на всей организации [Параметры > Внешний](https://admin.teams.microsoft.com/company-wide-settings/external-communications) доступ и включите "Пользователи могут общаться с Skype для бизнеса и Teams пользователями", а затем выполните все действия в Let [your Teams users chat and communicate with users in another organisation](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
