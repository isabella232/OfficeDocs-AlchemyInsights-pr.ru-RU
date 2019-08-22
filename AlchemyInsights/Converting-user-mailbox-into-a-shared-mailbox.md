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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="b0255-102">Преобразование почтового ящика пользователя в общий почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="b0255-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="b0255-103">Вы можете преобразовать почтовый ящик пользователя в общий почтовый ящик только в том случае, если у пользователя есть лицензия Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0255-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="b0255-104">После преобразования почтового ящика он по-прежнему будет отображаться в списке Активные пользователи, так как этот список содержит общие почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="b0255-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="b0255-105">Однако преобразованный почтовый ящик также будет отображаться в списке общих почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="b0255-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="b0255-106">При попытке преобразования почтового ящика в консоли администрирования Exchange в случае сбоя преобразования очистите кэш браузера и файлы cookie и повторите попытку.</span><span class="sxs-lookup"><span data-stu-id="b0255-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="b0255-107">Если она все еще не работает, попробуйте преобразовать почтовый ящик в командную консоль Exchange, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="b0255-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="b0255-108">Дополнительные сведения о преобразовании почтовых ящиков доступны при [преобразовании почтового ящика пользователя в общий почтовый ящик](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="b0255-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
