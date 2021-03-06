---
title: Управление ведением журнала
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510042"
---
# <a name="manage-journaling"></a><span data-ttu-id="37ffe-102">Управление ведением журнала</span><span class="sxs-lookup"><span data-stu-id="37ffe-102">Manage journaling</span></span>

<span data-ttu-id="37ffe-103">Функция ведения журнала позволяет организации соответствовать правовым, регулятивным и организационным требованиям, записывая все входящие и исходящие сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="37ffe-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="37ffe-104">Помните:</span><span class="sxs-lookup"><span data-stu-id="37ffe-104">Keep in mind:</span></span>

* <span data-ttu-id="37ffe-105">Для управления [журналами](https://go.microsoft.com/fwlink/?linkid=2115259) [](https://go.microsoft.com/fwlink/?linkid=2115469) необходимо иметь разрешения на управление организацией и управление записями.</span><span class="sxs-lookup"><span data-stu-id="37ffe-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="37ffe-106">Необходимо настроить почтовый ящик журнала и (необязательно) альтернативный почтовый ящик для журналов.</span><span class="sxs-lookup"><span data-stu-id="37ffe-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="37ffe-107">Дополнительные дополнительные ссылки см. [в журнале Configure Journaling in Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="37ffe-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="37ffe-108">В Exchange Online существует ограничение на количество правил журнала, которые можно создать.</span><span class="sxs-lookup"><span data-stu-id="37ffe-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="37ffe-109">Подробные сведения [см. в материале Ограничения правил "Журнал", "Транспорт" и "Входящие".](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="37ffe-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="37ffe-110">Exchange Online не поддерживает доставку отчетов журнала в почтовый ящик Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="37ffe-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="37ffe-111">В качестве почтового ящика журнала необходимо указать адрес электронной почты локальной системы архива или стороной службы архива.</span><span class="sxs-lookup"><span data-stu-id="37ffe-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
