---
title: Нужна помощь с лимитами отправки электронной почты?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702376"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="d7330-102">Нужна помощь с лимитами отправки электронной почты?</span><span class="sxs-lookup"><span data-stu-id="d7330-102">Need help with email sending limits?</span></span>

<span data-ttu-id="d7330-103">Ниже приведены **ограничения на отправку**, установленные в службе.</span><span class="sxs-lookup"><span data-stu-id="d7330-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="d7330-104">Больше информации об этих пределах документировано [здесь](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="d7330-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="d7330-105">Чтобы препятствовать доставке нежелательных массовых сообщений, мы применяем **ограничения скорости на каждого пользователя для всех исходящих и внутренних сообщений**.</span><span class="sxs-lookup"><span data-stu-id="d7330-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="d7330-106">Во всех SKU этот лимит составляет **10 000 получателей в день**.</span><span class="sxs-lookup"><span data-stu-id="d7330-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="d7330-107">Клиенты, которым необходимо отправлять законные массовые коммерческие электронные письма (например, информационные бюллетени), должны использовать сторонних поставщиков, которые специализируются на этих услугах.</span><span class="sxs-lookup"><span data-stu-id="d7330-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="d7330-108">**Примечание**: Как только предел скорости получателей достигнут, сообщения не могут отправляться из почтового ящика до тех пор, пока количество получателей, которым были отправлены сообщения за последние 24 часа, не упадет ниже этого предела.</span><span class="sxs-lookup"><span data-stu-id="d7330-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="d7330-109">Пользователь не сможет отправлять сообщения до этого момента.</span><span class="sxs-lookup"><span data-stu-id="d7330-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="d7330-110">Предел скорости сообщений **30 сообщений в минуту** применяется ко всем SKU.</span><span class="sxs-lookup"><span data-stu-id="d7330-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="d7330-111">Это определяет, сколько сообщений пользователь может отправить из своей учетной записи Exchange Online за указанный период.</span><span class="sxs-lookup"><span data-stu-id="d7330-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="d7330-112">**Максимальное количество получателей, допустимое в полях «Кому», «Копия» и «Скрытая копия»** для одного сообщения электронной почты во всех SKU, составляет **1000 получателей**.</span><span class="sxs-lookup"><span data-stu-id="d7330-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="d7330-113">Чтобы настроить этот лимит, перейдите [сюда](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="d7330-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
