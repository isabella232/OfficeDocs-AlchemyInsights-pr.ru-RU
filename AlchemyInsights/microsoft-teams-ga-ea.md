---
title: Microsoft Teams — гостевой доступ
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
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798389"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams — гостевой доступ

Если вам нужна помощь в обмене данными с пользователями, находящимися за пределами Организации в Teams, необходимо решить, следует ли использовать [гостевой доступ или внешний доступ (Федерацию)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), или можно использовать оба варианта.

[Ознакомьтесь с различиями](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) , чтобы узнать, какие функции доступны для каждой из них.  Например, внешний доступ (Федерация) поддерживает связь 1:1, например чат и присутствие.  Федеративные пользователи не могут участвовать в совместной работе в Teams, но.  Если вы хотите, чтобы внешний пользователь присоединяться к беседам по каналу Teams или совместно использовать файлы, необходимо включить гостевой доступ.

**Вариант 1: включение гостевого доступа**   
В центре администрирования Teams выберите параметры для [всей организации > гостевой доступ](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) и включите параметр "разрешить гостевой доступ в Teams".  Для клиента со всеми другими параметрами по умолчанию это все, что нужно сделать.  Чтобы настроить конфигурацию гостевого доступа, убедитесь, что выполнены все действия, описанные в [контрольном списке гостевого доступа](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Когда все будет готово, необходимо [подождать до 24 часов](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) , чтобы параметры вступили в силу.

Если вы уверены, что выполнили все действия, описанные в контрольном списке, и оно было более 24 часов, попробуйте [Добавить гостя в команду](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Для получения дополнительных сведений, включая видеоролики, ознакомьтесь со статьей [гостевой доступ в Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Вариант 2: включение внешнего доступа (Федерация)** Если вы также хотите включить внешний доступ (Федерацию), в центре администрирования Teams перейдите к параметрам, расположенным в [организации > внешний доступ](https://admin.teams.microsoft.com/company-wide-settings/external-communications) , и включите "пользователи могут общаться с пользователями Skype для бизнеса и Teams", а затем выполните все действия, описанные в разделе [Позвольте пользователям Teams общаться и общаться с пользователями в другой организации](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).


