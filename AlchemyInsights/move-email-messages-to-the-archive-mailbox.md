---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28309056"
---
Проблемы при архивации элементов в архивный почтовый ящик. Убедитесь в том, что выполнены следующие действия:
  
1. Убедитесь, что **архив почтового ящика** был включен. Если нет, выполните действия в [этой статье](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) , чтобы включить в архивный почтовый ящик. 
    
2. В центре администрирования Exchange выберите **Теги хранения** в разделе **Управление соответствием требованиям**, создайте **тега хранения** с действием **Переместить в архив** , содержащий желаемую **Срока хранения**.
    
3. В центре администрирования Exchange выберите **Политики хранения**, создайте **Политику хранения** и добавьте вашей **Переместить в архив** тега хранения для этой политики. 
    
4. [Назначение политики хранения](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для определенного пользователя почтового ящика. Та же политика будет применяться к **основной** и **архивного** почтового ящика. 
    
Почтовый ящик пользователя должны появиться политики архивирования для перемещаются в архивный почтовый ящик. Может потребоваться принудительно управляемых папок Assistant (многофакторной проверкой Подлинности) для запуска и применения новых параметров почтового ящика пользователя. Выполните следующую команду при [подключенной к EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) запуск помощника для управляемых папок для определенного почтового ящика: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Дополнительные сведения о настройке политики архивирования, к разделу [Set архива и удаления политики почтовых ящиков](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

