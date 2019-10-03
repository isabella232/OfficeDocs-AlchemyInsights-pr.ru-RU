---
title: Параметры политики собраний
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376796"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление политиками собраний в Microsoft Teams

Политики собраний используются для управления возможностями, доступными участникам собрания для собраний, запланированных пользователями в Организации. Некоторые функции политик собраний могут не быть реализованы в центре администрирования Teams, но они помечаются как "скоро" в документации. В этом случае, или если вы получаете сообщение об ошибке "не удается обновить политику, но повторите попытку позже" в центре администрирования Microsoft Teams, мы рекомендуем использовать PowerShell для создания или изменения политик собрания Teams. 

Дополнительные сведения о политиках собраний содержатся в следующих ресурсах:

- Чтобы узнать о создании политик, внесении изменений и назначении пользователям политики, ознакомьтесь со статьей [Управление политиками собраний в Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Чтобы изменить политику с помощью командлетов PowerShell, ознакомьтесь с разделом [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Необходимо использовать [модуль PowerShell Skype для бизнеса](https://www.microsoft.com/download/details.aspx?id=39366) для политик собраний Teams. 
    - Ознакомьтесь с [документацией по командлетам * – кстеамсмитингполици](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для получения дополнительных сведений.

**Примечание:** Для вступления в силу изменений политики для пользователей может потребоваться до 24 часов. Возможно, вы не сможете вносить изменения сразу для вновь созданных политик; Подождите 4 часа и попытайтесь изменить вновь созданную политику. Если у вас по-прежнему возникают проблемы, попробуйте использовать PowerShell.  