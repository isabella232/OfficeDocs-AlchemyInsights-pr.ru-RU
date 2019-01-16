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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308742"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Ошибка при отправке электронной почты: заблокировано с помощью Spamhaus узла клиента

IP-адрес, который отправляет сообщение — черного списка, владельцем которого [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Блокировка Spamhaus причины атаке учетные записи раскрыты машины, общий доступ к общедоступный IP-адрес и политики службы поставщика услуг Интернета. Приведены возможные исправления:
  
- Заблокированные входящие сообщения в Office 365, где можно управлять исходного сервера электронной почты необходимо определить причину и удалите блок Spamhaus веб-сайте.
    
- Заблокированные входящие сообщения в Office 365, где исходный IP-адрес принадлежит другому пользователю адрес владелец должен удалить блок Spamhaus веб-сайте. Если IP-адрес на списка блокировки политики (PBL), владелец можно назначить разные статический IP-адрес или удалите адрес из PBL.
    
- Заблокированные исходящих сообщений из домена Office 365 Эта ошибка может возникнуть, если сообщения направляются через службу сторонних производителей. Поиск владельцу адрес заблокированных IP-адресов можно использовать средство поиска WHOIS.
    

