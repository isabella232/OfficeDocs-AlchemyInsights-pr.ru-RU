---
title: Настройка автоматических ответов для почтового ящика
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046621"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Настройка автоматических ответов для почтового ящика пользователя

**Метод 1**

1. Войдите на портал Microsoft 365.

2. Выберите **Пользователи > Активные пользователи** (или **Группы > Общие почтовые ящики**, если выполняется настройка в общем почтовом ящике).

3. Выберите пользователя, у которого есть почтовый ящик Microsoft Exchange.

4. Во всплывающем меню справа выберите **Параметры почты > Автоматические ответы** (если это общий почтовый ящик, просто щелкните **Автоматические ответы** во всплывающем меню).

**Метод 2**

1. Войдите на портал администрирования Microsoft 365, используя учетные данные администратора.

2. Разверните пункт **Центры администрирования** и щелкните **Exchange**.

3. Щелкните изображение в правом верхнем углу, нажмите **Еще один пользователь** и выберите почтовый ящик пользователя, который нужно изменить.

4. В левой части выберите **Параметры**, щелкните **Упорядочить электронную почту** и нажмите **Автоматические ответы**.

**Метод 3**

В Exchange Online PowerShell выполните следующий командлет:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Дополнительные сведения об этом командлете см. в статье [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
