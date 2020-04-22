---
title: Ошибка при отправке сообщения, заблокированного Спамхаус
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714271"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="6ec03-102">Ошибка при отправке сообщения: узел клиента заблокирован с помощью Спамхаус</span><span class="sxs-lookup"><span data-stu-id="6ec03-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="6ec03-103">IP-адрес, который отправил сообщение, находится в черном списке, принадлежащем [спамхаус](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="6ec03-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="6ec03-104">Причины блокирования Спамхаус включают скомпрометированные учетные записи, зараженные компьютеры, совместно использующих общедоступный IP-адрес, а также политики поставщика услуг Интернета.</span><span class="sxs-lookup"><span data-stu-id="6ec03-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="6ec03-105">Возможные исправления:</span><span class="sxs-lookup"><span data-stu-id="6ec03-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="6ec03-106">Для заблокированных входящих сообщений, в которых вы контролируете исходный сервер электронной почты, необходимо определить причину и удалить блок с веб-сайта Спамхаус.</span><span class="sxs-lookup"><span data-stu-id="6ec03-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="6ec03-107">Для заблокированных входящих сообщений, в которых исходный IP-адрес принадлежит другому пользователю, владельцу адреса необходимо удалить этот блок с веб-сайта Спамхаус.</span><span class="sxs-lookup"><span data-stu-id="6ec03-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="6ec03-108">Если IP-адрес находится в списке блокировок политик (ПБЛ), владелец может назначить другой статический IP-адрес или удалить адрес из ПБЛ.</span><span class="sxs-lookup"><span data-stu-id="6ec03-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="6ec03-109">Для заблокированных исходящих сообщений из вашего домена, подключенного к корпорации Майкрософт, вы можете получить эту ошибку, если сообщения маршрутизируются через сторонние службы.</span><span class="sxs-lookup"><span data-stu-id="6ec03-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="6ec03-110">Вы можете использовать средство поиска WHOIS, чтобы найти владельца заблокированного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="6ec03-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
