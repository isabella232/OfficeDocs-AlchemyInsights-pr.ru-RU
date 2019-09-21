---
title: Исходящая почта в папке нежелательной почты
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062828"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="38e3f-102">Исходящая почта в папке нежелательной почты</span><span class="sxs-lookup"><span data-stu-id="38e3f-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="38e3f-103">Если вы видите исходящие сообщения, помеченные как нежелательные, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="38e3f-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="38e3f-104">Если вы еще не сделали это, рассмотрите вопрос [о настройке уведомлений политики нежелательной почты](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="38e3f-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="38e3f-105">Используйте [трассировку сообщений](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) , чтобы узнать, содержит ли исходящее сообщение значение события **спама** , с дополнительным описанием. **Используйте пул доставки с высоким уровнем риска**.</span><span class="sxs-lookup"><span data-stu-id="38e3f-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="38e3f-106">Для этих сообщений просмотрите содержимое сообщения, чтобы узнать, что может считаться нежелательной почтой.</span><span class="sxs-lookup"><span data-stu-id="38e3f-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="38e3f-107">Например, подписи иногда могут вызывать проблемы для многих пользователей.</span><span class="sxs-lookup"><span data-stu-id="38e3f-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="38e3f-108">Если у вас несколько примеров допустимых исходящих сообщений, помеченных как нежелательная почта, откройте билет в службу поддержки и попросите агента службы поддержки отправлять сообщения в качестве ложных срабатываний в аналитиках нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="38e3f-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="38e3f-109">Будьте готовы к предоставлению образцов сообщений, включающих все заголовки сообщений.</span><span class="sxs-lookup"><span data-stu-id="38e3f-109">Be prepared to provide sample messages that include all message headers.</span></span>
