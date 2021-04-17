---
title: Невозможно получить доступ к общедоступным папкам
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819525"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не может подключаться к общедоступным папкам

Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте следующее:

Подключись к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox в учетной записи пользователя проблемы, чтобы соответствовать параметру рабочей учетной записи пользователя.

Пример.

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Подождите по крайней мере один час, пока изменение вступает в силу.

Если проблема сохраняется, выполните эту [процедуру,](https://aka.ms/pfcte) чтобы устранить проблемы с доступом к общедоступным папам с помощью Outlook.
 
**Управление доступом пользователей к общедоступным папкам с помощью Outlook:**

1.  Используйте <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true или $false  
      
    $true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
      
    $false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Примечание** Эта процедура может управлять подключениями только с настольным компьютером Outlook для клиентов Windows. Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.
 
Дополнительные сведения см. в анонсе "Поддержка контролируемых подключений к [общедоступным папкам в Outlook".](https://aka.ms/controlpf)