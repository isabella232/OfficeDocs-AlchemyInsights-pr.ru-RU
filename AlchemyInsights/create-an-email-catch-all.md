---
title: Создание улова электронной почты
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816213"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="23468-102">Создание улова электронной почты</span><span class="sxs-lookup"><span data-stu-id="23468-102">Create an email catch all</span></span>

<span data-ttu-id="23468-103">Использование улова все настоятельно рекомендуется.</span><span class="sxs-lookup"><span data-stu-id="23468-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="23468-104">Лучше предоставить отскок отправителю, позволяя отправителям знать, что их сообщение не может быть доставлено по мере решения, чтобы они могли принять меры.</span><span class="sxs-lookup"><span data-stu-id="23468-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="23468-105">Вы также можете ограничить отслеживаемую почту только для того, чтобы ловить ранее допустимые адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="23468-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="23468-106">Любой улов всех почтовых ящиков будет получать много нежелательной почты и может в конечном итоге заполнить, если не внимательно следить.</span><span class="sxs-lookup"><span data-stu-id="23468-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="23468-107">(Существуют ограничения на получение.)</span><span class="sxs-lookup"><span data-stu-id="23468-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="23468-108">Если вы решите продолжить, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="23468-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="23468-109">Создание группы динамического распространения & "Все типы получателей".</span><span class="sxs-lookup"><span data-stu-id="23468-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="23468-110">Создайте специальный почтовый ящик для ловли электронных писем, например, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="23468-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="23468-111">Для определенного домена установите DomainType на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="23468-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="23468-112">Если вы позже удалите все уловы, не забудьте установить домен обратно в Авторитетный.</span><span class="sxs-lookup"><span data-stu-id="23468-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="23468-113">Создайте правило транспорта почтового потока следующим образом:</span><span class="sxs-lookup"><span data-stu-id="23468-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="23468-114">Если отправитель "Вне организации"</span><span class="sxs-lookup"><span data-stu-id="23468-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="23468-115">Перенаправление сообщения на Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="23468-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="23468-116">Кроме того, что получатель является членом allusers@domain.com (Группа рассылки содержит всех участников)</span><span class="sxs-lookup"><span data-stu-id="23468-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="23468-117">Убедитесь, что новые почтовые ящики добавлены в группу динамического распространения</span><span class="sxs-lookup"><span data-stu-id="23468-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
