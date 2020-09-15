---
title: Создание сообщения "перехватывать все"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712999"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="8d96b-102">Создание сообщения "перехватывать все"</span><span class="sxs-lookup"><span data-stu-id="8d96b-102">Create an email catch all</span></span>

<span data-ttu-id="8d96b-103">Не рекомендуется использовать catch ALL.</span><span class="sxs-lookup"><span data-stu-id="8d96b-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="8d96b-104">Лучше предоставить отправителю сообщение о том, что сообщение не было доставлено как адресованное, чтобы они могли предпринять действия.</span><span class="sxs-lookup"><span data-stu-id="8d96b-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="8d96b-105">Вы также можете ограничить отслеживаемые почтовые ящики только ранее допустимыми адресами электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8d96b-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="8d96b-106">Любой захватывать все почтовые ящики будут получать ценные сообщения о нежелательной почте и, в конце концов, могут заполняться.</span><span class="sxs-lookup"><span data-stu-id="8d96b-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="8d96b-107">(Существуют пределы получения).</span><span class="sxs-lookup"><span data-stu-id="8d96b-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="8d96b-108">Если вы решили продолжить, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="8d96b-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="8d96b-109">Создайте динамическую группу рассылки & включить "все типы получателей".</span><span class="sxs-lookup"><span data-stu-id="8d96b-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="8d96b-110">Создание выделенного почтового ящика для перехвата сообщений электронной почты, например catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="8d96b-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="8d96b-111">Для определенного домена задайте для параметра Домаинтипе значение "Интерналрелай".</span><span class="sxs-lookup"><span data-stu-id="8d96b-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="8d96b-112">Если после этого вы удалите все данные, убедитесь, что в качестве домена выбрано значение заслуживающий доверия.</span><span class="sxs-lookup"><span data-stu-id="8d96b-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="8d96b-113">Создайте правило транспорта Mailflow следующим образом:</span><span class="sxs-lookup"><span data-stu-id="8d96b-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="8d96b-114">Если отправитель — "за преходящей организацией"</span><span class="sxs-lookup"><span data-stu-id="8d96b-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="8d96b-115">Перенаправление сообщения в Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="8d96b-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="8d96b-116">Кроме случая, когда получатель является членом allusers@domain.com (группа рассылки содержит всех участников)</span><span class="sxs-lookup"><span data-stu-id="8d96b-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="8d96b-117">Проверка того, что новые почтовые ящики добавляются в динамическую группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="8d96b-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
