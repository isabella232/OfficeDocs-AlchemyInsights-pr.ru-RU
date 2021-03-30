---
title: Проверка на пересылку адресов в почтовых ящиках
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403324"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="eb22e-102">Проверка на пересылку адресов в почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="eb22e-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="eb22e-103">Иногда хакеры пересылают сообщения электронной почты пользователей самим себе, поэтому сначала мы проверяем, как пересылать адреса и правила в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="eb22e-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="eb22e-104">Затем мы проверим журналы аудита.</span><span class="sxs-lookup"><span data-stu-id="eb22e-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="eb22e-105">Вот как проверить, как переададовать адреса:</span><span class="sxs-lookup"><span data-stu-id="eb22e-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="eb22e-106">Выбор **пользователей**  >  **Активные пользователи**.</span><span class="sxs-lookup"><span data-stu-id="eb22e-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="eb22e-107">Выберите пользователя, чья учетная запись скомпрометирована.</span><span class="sxs-lookup"><span data-stu-id="eb22e-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="eb22e-108">В вылете, который появляется, раздвигать **параметры почты,** а затем нажмите **кнопку Изменить** для **пересылания электронной почты**.</span><span class="sxs-lookup"><span data-stu-id="eb22e-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="eb22e-109">Удалите не распознающие адреса переададки.</span><span class="sxs-lookup"><span data-stu-id="eb22e-109">Remove any forwarding addresses you don't recognize.</span></span>