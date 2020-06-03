---
title: Исходящая почта в папке нежелательной почты
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511737"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="ac0a6-102">Исходящая почта в папке нежелательной почты</span><span class="sxs-lookup"><span data-stu-id="ac0a6-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="ac0a6-103">Если вы видите исходящие сообщения, помеченные как нежелательные, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="ac0a6-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="ac0a6-104">Если вы еще не сделали это, рассмотрите вопрос [о настройке уведомлений политики нежелательной почты](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="ac0a6-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="ac0a6-105">Используйте [трассировку сообщений](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , чтобы узнать, содержит ли исходящее сообщение значение события **спама** , с дополнительным описанием. **Используйте пул доставки с высоким уровнем риска**.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="ac0a6-106">Для этих сообщений просмотрите содержимое сообщения, чтобы узнать, что может считаться нежелательной почтой.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="ac0a6-107">Например, подписи иногда могут вызывать проблемы для многих пользователей.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="ac0a6-108">Если у вас несколько примеров допустимых исходящих сообщений, помеченных как нежелательная почта, откройте билет в службу поддержки и попросите агента службы поддержки отправлять сообщения в качестве ложных срабатываний в аналитиках нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="ac0a6-109">Будьте готовы к предоставлению образцов сообщений, включающих все заголовки сообщений.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-109">Be prepared to provide sample messages that include all message headers.</span></span>
