---
title: Применение ограничений на получение к почтовому ящику
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829159"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Применение ограничений на получение к почтовому ящику

Недавно корпорация Майкрософт начала применять ограничение для каждого почтового ящика в размере 3600 сообщений в час. Дополнительные сведения см. в статье [Ограничения Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). К почтовым ящикам Microsoft 365, которые получают более 3600 сообщений в течение часа, применяются ограничения в течение следующих 60 минут. 

Кроме того, применяется ограничение к паре отправитель-получатель (SRP), которое блокирует получение почтовым ящиком Microsoft 365 сообщений от конкретного отправителя. Если один отправитель отправляет более 33% сообщений от общего порогового значения или 1200 сообщений в час конкретному получателю, то в отношении него вступает в силу ограничение SRP, и почтовый ящик больше не принимает сообщения от этого отправителя. Обратите внимание на следующее.

- Это ограничение применяется к электронным письмам, полученным от других клиентов, локальных отправителей или отправителей в Интернете.
- Доставка электронных писем в почтовый ящик блокируется в на следующие 60 минут. 
- Отправители, которые отправляют сообщения электронной почты в эти почтовые ящики, получают отчет о недоставке (5.2.121 или 5.2.122) с указанием того, что почтовый ящик превысил максимальный порог доставки сообщений. Сообщения внутри клиента (почтовый ящик в том же клиенте) по-прежнему продолжат доставляться.
- Когда применяется ограничение SRP, почтовые ящики-получатели продолжают принимать сообщения от других отправителей.

Администраторы могут отслеживать текущую активность почтовых ящиков, перейдя к новому отчету или аналитике в Центре администрирования Exchange под названием "Почтовые ящики, превышающие ограничения на получение". Аналитика отображается только в том случае, если в клиенте присутствуют проблемные почтовые ящики, а отчет всегда выводится на панель мониторинга, но будет пустым, если в клиенте присутствуют проблемные почтовые ящики.

Дополнительные сведения об аналитике, касающейся ограничений на получение, см. в разделе [Аналитика нового Центра администрирования Exchange о превышении лимитов получения в почтовых ящиках](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Дополнительные сведения об отчете о превышении ограничений на получение см. в разделе [Отчет нового Центра администрирования Exchange о превышении лимитов получения в почтовых ящиках.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)