---
title: Использование стикерами в беседах в Teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947513"
---
# <a name="using-giphys-in-teams-conversations"></a>Использование стикерами в беседах в Teams

Стикерами доступ в чате в Teams включен по умолчанию. Как администратор вы можете контролировать доступность стикерами для пользователей, [настроив политику обмена сообщениями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) и убедившись в **том, что** **Использование стикерами в беседах** включено.

Если GIF в беседах Teams не работает должным образом, убедитесь, что:

[Политика обмена сообщениями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) должна разрешить стикерами. Чтобы проверить с помощью командлетов PowerShell, выполните следующие действия:

- Убедитесь, что вы можете [управлять Teams с помощью PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Выполните команду PowerShell [Get-кстеамсмессагингполици-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и убедитесь, что для **Алловгифи** задано **значение true**.
- Если для **алловгифи** задано **значение false** , выполните следующую команду PowerShell [Set-Кстеамсмессагингполици-Identity global-алловгифи $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Для предоставления доступа к URL-адресу Giphy необходимо включить [необязательный подключенный интерфейс](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Если для клиента настроено несколько политик обмена сообщениями Teams, можно определить удостоверение политики, назначенной для затронутого пользователя, с помощью команды PowerShell [Get – CsOnlineUser – Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Выберите Теамсмессагингполици.
