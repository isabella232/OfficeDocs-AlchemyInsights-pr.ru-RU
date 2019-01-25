---
title: Преобразование почтовых ящиков пользователей в общем почтовом ящике?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486218"
---
<span data-ttu-id="36b62-p101">Почтовый ящик пользователя можно преобразовать к общему почтовому ящику, только если у пользователя есть лицензии Exchange. После преобразования почтовый ящик будет продолжать отображаться в список активных пользователей, так как этот список включает в себя общие почтовые ящики. Тем не менее преобразованные почтового ящика будет также отображаться в списке общего почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="36b62-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="36b62-p102">При попытке преобразования почтового ящика в консоли администрирования Exchange и не удается выполнить преобразование, очистите кэш браузера и файлы cookie и повторите попытку. Если он все еще не работает, попробуйте выполните преобразование почтовых ящиков в командной консоли Exchange, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="36b62-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="36b62-107">Дополнительные сведения о почтовых ящиках преобразования доступна в [Преобразование почтового ящика пользователя к общему почтовому ящику](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="36b62-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
