---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341416"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не удается подключиться к общедоступным папкам

Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте выполнить следующие действия:

Подключитесь к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox учетной записи пользователя, чтобы он был сопоставлен с параметром рабочей учетной записи пользователя.

Пример.

Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс

Set — Mailbox Проблемусер — DefaultPublicFolderMailbox \<value from previous command>

Чтобы изменения вступили в силу, подождите хотя бы один час.

Если проблема не устранена, выполните указанные ниже [действия](https://aka.ms/pfcte) , чтобы устранить проблемы с доступом к общим папкам с помощью Outlook.
 
**Чтобы определить, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook**:

1.  Используйте Set – CASMailbox <mailboxname> публикфолдерклиентакцесс $true или $false  
      
    $true: разрешить пользователям доступ к общедоступным папкам в Outlook  
      
    $false: запретить пользователям доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  
        
2.  Set — OrganizationConfig — Публикфолдершовклиентконтрол $true   
      
**Note (Примечание** ) Эта процедура позволяет управлять подключениями только с клиентами Outlook Desktop для Windows. Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.
 
Дополнительные сведения приведены в статье [объявления о поддержке управляемых подключений для общедоступных папок в Outlook](https://aka.ms/controlpf).