---
title: Ошибка входа в Teams адресации AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953048"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Ошибка входа в Teams адресации AADSTS9000411

При входе в Microsoft Teams вы можете получить сообщение об ошибке: **Извините, но у нас возникли проблемы с подписью вас в AADSTS9000411: запрос неправильно отформатирован. Параметр "login_hint" дублируется.**

Чтобы решить эту проблему, убедитесь, что ваши клиенты Microsoft Teams обновлены. Для получения дополнительной информации об обновлении вашего клиента см. [Обновление Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Если по какой-то причине вы не можете обновить свой клиент, выход из него приведет к удалению большинства кэшированных данных. Однако, если у вас все еще есть проблемы после выхода/входа из системы, выйдите из Teams и очистите кэш клиента, выполнив следующие действия:
1. Закройте Microsoft Teams.
2. Перейдите по адресу:%appdata%\microsoft\teams и удалите все файлы.
3. Снова откройте Microsoft Teams.
