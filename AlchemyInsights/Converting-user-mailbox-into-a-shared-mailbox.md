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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374336"
---
<span data-ttu-id="09ecb-102">Вы можете преобразовать почтовый ящик пользователя в общий почтовый ящик только в том случае, если у пользователя есть лицензия Exchange.</span><span class="sxs-lookup"><span data-stu-id="09ecb-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="09ecb-103">После преобразования почтового ящика он по-прежнему будет отображаться в списке Активные пользователи, так как этот список содержит общие почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="09ecb-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="09ecb-104">Однако преобразованный почтовый ящик также будет отображаться в списке общих почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="09ecb-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="09ecb-105">При попытке преобразования почтового ящика в консоли администрирования Exchange в случае сбоя преобразования очистите кэш браузера и файлы cookie и повторите попытку.</span><span class="sxs-lookup"><span data-stu-id="09ecb-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="09ecb-106">Если она все еще не работает, попробуйте преобразовать почтовый ящик в командную консоль Exchange, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="09ecb-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="09ecb-107">Дополнительные сведения о преобразовании почтовых ящиков доступны при [преобразовании почтового ящика пользователя в общий почтовый ящик](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="09ecb-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
