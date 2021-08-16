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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996643"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не удается подключиться к общедоступным папкам

Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте следующее:

Подключение EXO PowerShell и настройте параметр DefaultPublicFolderMailbox в проблемной учетной записи пользователя, чтобы соответствовать параметру рабочей учетной записи пользователя.

Пример:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Подождите по крайней мере один час, пока изменение вступает в силу.

Если проблема сохраняется, [](https://aka.ms/pfcte) выполните эту процедуру, чтобы устранить проблемы с доступом к общедоступным папкам с помощью Outlook.
 
**Чтобы контролировать, какие пользователи могут получать доступ к общедоступным папкам с Outlook:**

1.  Используйте <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true или $false  
      
    $true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
      
    $false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Примечание** Эта процедура может управлять подключениями только с Outlook для Windows клиентов. Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.
 
Дополнительные сведения см. в сайте [Announcing Support for Controlled Connections to Public Folders in Outlook.](https://aka.ms/controlpf)