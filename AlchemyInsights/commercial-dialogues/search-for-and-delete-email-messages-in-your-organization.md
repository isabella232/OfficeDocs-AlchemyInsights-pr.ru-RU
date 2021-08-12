---
title: Поиск и удаление сообщений электронной почты в вашей организации
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948896"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Поиск и удаление сообщений электронной почты в вашей организации

Выполните приведенные ниже действия.

1. Если вы не глобальный администратор, для поиска сообщений ваша учетная запись должна быть добавлена в группу ролей **диспетчера** электронных поисков или роль управления поиском **соответствия** требованиям. Чтобы удалить сообщения, необходимо присоединиться к группе ролей **управления** организацией или роли управления поиском и **очисткой.** Разрешения на эти роли назначены в центре [& соответствия требованиям.](https://protection.office.com)
2. [Создайте поиск контента,](https://docs.microsoft.com/office365/securitycompliance/content-search) чтобы найти удаление сообщения.
3. [Подключитесь к Центру безопасности и соответствия требованиям PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Если вы используете MFA, см. в этих инструкциях: Подключение службе безопасности & PowerShell с помощью [многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Удаление сообщения: запустите `New-ComplianceSearchAction` cmdlet, чтобы удалить сообщение. Удаленные сообщения перемещаются в папку "Извлекаемые элементы" пользователя. Пример команды см. в [шаге 3. Удаление сообщения.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
