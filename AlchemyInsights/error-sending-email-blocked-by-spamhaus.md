---
title: Ошибка при отправке электронной почты, блокирует SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486209"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d1224-102">Ошибка при отправке электронной почты: заблокировано с помощью Spamhaus узла клиента</span><span class="sxs-lookup"><span data-stu-id="d1224-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d1224-p101">IP-адрес, который отправляет сообщение — черного списка, владельцем которого [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Блокировка Spamhaus причины атаке учетные записи раскрыты машины, общий доступ к общедоступный IP-адрес и политики службы поставщика услуг Интернета. Приведены возможные исправления:</span><span class="sxs-lookup"><span data-stu-id="d1224-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="d1224-106">Заблокированные входящие сообщения в Office 365, где можно управлять исходного сервера электронной почты необходимо определить причину и удалите блок Spamhaus веб-сайте.</span><span class="sxs-lookup"><span data-stu-id="d1224-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="d1224-p102">Заблокированные входящие сообщения в Office 365, где исходный IP-адрес принадлежит другому пользователю адрес владелец должен удалить блок Spamhaus веб-сайте. Если IP-адрес на списка блокировки политики (PBL), владелец можно назначить разные статический IP-адрес или удалите адрес из PBL.</span><span class="sxs-lookup"><span data-stu-id="d1224-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="d1224-p103">Заблокированные исходящих сообщений из домена Office 365 Эта ошибка может возникнуть, если сообщения направляются через службу сторонних производителей. Поиск владельцу адрес заблокированных IP-адресов можно использовать средство поиска WHOIS.</span><span class="sxs-lookup"><span data-stu-id="d1224-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

