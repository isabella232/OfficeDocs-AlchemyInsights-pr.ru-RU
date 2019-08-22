---
title: Преобразование почтового ящика пользователя в общий почтовый ящик
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496448"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Преобразование почтового ящика пользователя в общий почтовый ящик

Вы можете преобразовать почтовый ящик пользователя в общий почтовый ящик только в том случае, если у пользователя есть лицензия Exchange. После преобразования почтового ящика он по-прежнему будет отображаться в списке Активные пользователи, так как этот список содержит общие почтовые ящики. Однако преобразованный почтовый ящик также будет отображаться в списке общих почтовых ящиков. 
  
При попытке преобразования почтового ящика в консоли администрирования Exchange в случае сбоя преобразования очистите кэш браузера и файлы cookie и повторите попытку. Если она все еще не работает, попробуйте преобразовать почтовый ящик в командную консоль Exchange, выполнив следующую команду:
  
```
Set-Mailbox -Type Shared
```

Дополнительные сведения о преобразовании почтовых ящиков доступны при [преобразовании почтового ящика пользователя в общий почтовый ящик](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
