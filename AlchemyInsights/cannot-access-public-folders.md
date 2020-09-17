---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812560"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не удается подключиться к общедоступным папкам

Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте выполнить следующие действия:

Подключитесь к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox учетной записи пользователя, чтобы он был сопоставлен с параметром рабочей учетной записи пользователя.

Пример:

Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс

Set — Mailbox Проблемусер — DefaultPublicFolderMailbox \<value from previous command>

Чтобы изменения вступили в силу, подождите хотя бы один час.

Если проблема не устранена, выполните указанные ниже [действия](https://aka.ms/pfcte) , чтобы устранить проблемы с доступом к общим папкам с помощью Outlook.
 
**Чтобы определить, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook**:

1.  Используйте Set – CASMailbox <mailboxname> публикфолдерклиентакцесс $true или $false  
      
    $true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
      
    $false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  
        
2.  Set — OrganizationConfig — Публикфолдершовклиентконтрол $true   
      
**Note (Примечание** ) Эта процедура позволяет управлять подключениями только с клиентами Outlook Desktop для Windows. Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.
 
Дополнительные сведения приведены в статье [объявления о поддержке управляемых подключений для общедоступных папок в Outlook](https://aka.ms/controlpf).