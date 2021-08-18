---
title: Использование Giphys в Teams беседах
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323533"
---
# <a name="using-giphys-in-teams-conversations"></a>Использование Giphys в Teams беседах

Доступ giphys в Teams чате включен по умолчанию. Как администратор вы можете контролировать, доступны ли giphys пользователям, установив политику обмена сообщениями и обеспечив использование **Giphys** в беседах [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) **on**.

Если GIF-ы работают не так, как Teams беседах, убедитесь:

Политика [обмена сообщениями должна](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) разрешить Giphys. Проверка с помощью cmdlets PowerShell:

- Убедитесь, что [вы можете управлять Teams с PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Запустите команду PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и убедитесь, что **AllowGiphy** задает **true**.
- Если **allowGiphy** задает **false,** запустите следующую команду PowerShell [Set-CsTeamsMessagingPolicy-Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Чтобы разрешить](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) доступ к URL-адресу Giphy, необходимо включить необязательные подключенные функции.

**Примечание.** Если для клиента настроено несколько политик Teams обмена сообщениями, вы можете определить удостоверение политики, назначенной влияемому пользователю с помощью команды [PowerShell Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Выберите TeamsMessagingPolicy.
