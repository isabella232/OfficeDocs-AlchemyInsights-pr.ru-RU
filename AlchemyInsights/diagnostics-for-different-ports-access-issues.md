---
title: Диагностика различных проблем с доступом к портам
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030915"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Диагностика различных проблем с доступом к портам

Чтобы устранить различные проблемы с доступом к портам, выполните следующие действия.

1. Остановите или отмените выделение виртуальной машины (ВМ) на портале, перезапустите ВМ и проверьте снова. 
2. Проверьте сетевые параметры ВМ и выясните, есть ли у вас группы безопасности сети, блокирующие трафик. Вы также можете использовать [средство проверки IP-потока в составе Наблюдателя за сетями](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) для обнаружения групп безопасности сети, блокирующих трафик, заданных пользователями маршрутов, которые перенаправляют трафик обратно в локальное устройство ("Маршрут по умолчанию" 0.0.0.0/0) или на сетевое устройство.
Если после выполнения этих действий проблемы не исчезают, укажите имя виртуальной машины и TCP-порт, на которые вы пытаетесь отправить почту, для дальнейшей диагностики.

**Рекомендуемые документы**

[Ограничения и рекомендации по отправке исходящей электронной почты через порт 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)