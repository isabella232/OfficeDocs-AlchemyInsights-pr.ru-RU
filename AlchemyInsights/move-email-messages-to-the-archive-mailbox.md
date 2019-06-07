---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762378"
---
# <a name="move-email-to-the-archive-mailbox"></a>Перемещение электронной почты в архивный почтовый ящик
 
1. Убедитесь, что **архивный почтовый ящик** включен. В противном случае выполните действия, описанные в [этой статье](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , чтобы включить архивный почтовый ящик.

2. Чтобы автоматически архивировать сообщения в архивный почтовый ящик, тег хранения с действием **переместить в архив** должен **автоматически применять ко всему тегу почтового ящика (по умолчанию)**. Выполните действия, описанные в этой статье, чтобы создать тег: [Archive Default Tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Затем добавьте тег **Archive** в политику хранения. В центре администрирования Exchange выберите **политики хранения** > добавить **тег "переместить в архив** " в политику > **сохранить**. 
    
4. Теперь [назначьте политику хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для почтового ящика определенного пользователя. Та же политика будет применяться и к основному **** , и к **архивному** почтовому ящику. 
    
Может потребоваться принудительно запустить помощник по обслуживанию управляемых папок (MFA) и применить новые параметры к почтовому ящику пользователя. Выполните следующую команду при [подключении к EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) для запуска помощника по работе с управляемыми папками для определенного почтового ящика: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Дополнительные сведения о настройке политики архивации можно найти в разделе [Настройка политики архивации и удаления для](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)почтовых ящиков.
  

