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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737698"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Поиск и удаление сообщений электронной почты в вашей организации

Выполните следующие действия.

1. Если вы не глобальный администратор, для поиска сообщений ваша учетная запись должна быть добавлена в группу ролей **диспетчера** электронных поисков или роль управления поиском **соответствия** требованиям. Чтобы удалить сообщения, необходимо присоединиться к группе ролей **управления** организацией или роли управления поиском и **очисткой.** Разрешения на эти роли назначены в центре [& соответствия требованиям.](https://protection.office.com)
2. [Создайте поиск контента,](https://docs.microsoft.com/office365/securitycompliance/content-search) чтобы найти удаление сообщения.
3. [Подключитесь к Центру безопасности и соответствия требованиям PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Если вы используете MFA, см. в этих инструкциях: Подключение к центру & безопасности PowerShell с помощью [многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Удаление сообщения: запустите `New-ComplianceSearchAction` cmdlet, чтобы удалить сообщение. Удаленные сообщения перемещаются в папку "Извлекаемые элементы" пользователя. Пример команды см. в [шаге 3. Удаление сообщения.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
