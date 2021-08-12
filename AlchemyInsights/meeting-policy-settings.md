---
title: Параметры политик собраний
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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925178"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление политиками собраний в Microsoft Teams

**Примечание. Изменение политики для пользователей может занять до 24 часов.** Возможно, вы не сможете немедленно внести изменения в вновь созданные политики; подождите 4 часа и снова попытайтесь изменить вновь созданную политику.

Политики собраний используются для управления функциями, которые доступны участникам собрания для собраний, запланированных пользователями в вашей организации. Некоторые функции политик собраний пока не могут быть реализованы в центре администрирования Teams (в документации они помечены как "скоро"). В этом случае или при получении ошибки типа "Мы не можем обновить политику прямо сейчас, но попробуйте ее еще раз" в центре администрирования Microsoft Teams, рекомендуется использовать PowerShell для создания или изменения политик Teams собраний. 

Дополнительные сведения о политиках собраний см. в следующих ресурсах:

- Дополнительные новости о создании политик, внесении изменений и назначении пользователей политике см. в [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Чтобы изменить политику с помощью cmdlets PowerShell, [см. Teams Обзор PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Для политик собраний Skype для бизнеса PowerShell Teams модуль [powerShell.](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 
    - Дополнительные сведения см. в документации по [cmdlets *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

