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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897874"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="aed90-102">Диагностика различных проблем с доступом к портам</span><span class="sxs-lookup"><span data-stu-id="aed90-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="aed90-103">Чтобы устранить различные проблемы с доступом к портам, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="aed90-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="aed90-104">Остановите или отмените выделение виртуальной машины (ВМ) на портале, перезапустите ВМ и проверьте снова.</span><span class="sxs-lookup"><span data-stu-id="aed90-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="aed90-105">Проверьте сетевые параметры ВМ и выясните, есть ли у вас группы безопасности сети, блокирующие трафик.</span><span class="sxs-lookup"><span data-stu-id="aed90-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="aed90-106">Вы также можете использовать [средство проверки IP-потока в составе Наблюдателя за сетями](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) для обнаружения групп безопасности сети, блокирующих трафик, заданных пользователями маршрутов, которые перенаправляют трафик обратно в локальное устройство ("Маршрут по умолчанию" 0.0.0.0/0) или на сетевое устройство.</span><span class="sxs-lookup"><span data-stu-id="aed90-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="aed90-107">Если после выполнения этих действий проблемы не исчезают, укажите имя виртуальной машины и TCP-порт, на которые вы пытаетесь отправить почту, для дальнейшей диагностики.</span><span class="sxs-lookup"><span data-stu-id="aed90-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="aed90-108">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="aed90-108">**Recommended Documents**</span></span>

[<span data-ttu-id="aed90-109">Ограничения и рекомендации по отправке исходящей электронной почты через порт 25</span><span class="sxs-lookup"><span data-stu-id="aed90-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)