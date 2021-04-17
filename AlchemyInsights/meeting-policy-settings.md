---
title: Параметры политики собраний
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825456"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление политиками собраний в Microsoft Teams

**Примечание. Изменение политики для пользователей может занять до 24 часов.** Возможно, вы не сможете немедленно внести изменения в вновь созданные политики; подождите 4 часа и снова попытайтесь изменить вновь созданную политику.

Политики собраний используются для управления функциями, доступными участникам собраний для собраний, запланированных пользователями в организации. Некоторые функции политик собраний пока не могут быть реализованы в центре администрирования Teams (они помечены как "скоро" в документации). В этом случае или при получении ошибки типа "Мы не можем обновить политику прямо сейчас, но попробуйте ее еще раз" в центре администрирования Microsoft Teams, рекомендуется использовать PowerShell для создания или изменения политик собраний Teams. 

Дополнительные сведения о политиках собраний см. в следующих ресурсах:

- Чтобы узнать о создании политик, внесении изменений и назначении пользователей политике, см. в руб. Управление политиками [собраний в Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Чтобы изменить политику с помощью командлетов PowerShell, см. в обзоре [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Для политик собраний Teams необходимо использовать модуль Skype для бизнеса [PowerShell.](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 
    - Дополнительные сведения см. в документации по [cmdlets *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

