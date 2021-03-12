---
title: Набор реплик
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716278"
---
# <a name="replica-set"></a><span data-ttu-id="fe54a-102">Набор реплик</span><span class="sxs-lookup"><span data-stu-id="fe54a-102">Replica set</span></span>

<span data-ttu-id="fe54a-103">AADDS также называется управляемым доменом.</span><span class="sxs-lookup"><span data-stu-id="fe54a-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="fe54a-104">На самом деле это два контроллера домена, которые запускаются и поддерживаются backend.</span><span class="sxs-lookup"><span data-stu-id="fe54a-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="fe54a-105">Два DCs включают один основной DC и один DC репликации.</span><span class="sxs-lookup"><span data-stu-id="fe54a-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="fe54a-106">Резервное копирование в AADDS (управляемом домене) — это автоматизированный процесс, управляемый платформой Azure.</span><span class="sxs-lookup"><span data-stu-id="fe54a-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="fe54a-107">В случае проблемы с управляемым доменом поддержка Azure может помочь вам в восстановлении из резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="fe54a-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="fe54a-108">Каждая реплика создается в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="fe54a-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="fe54a-109">Каждая виртуальная сеть должна быть вглядеться во все другие виртуальные сети, в которых размещен набор реплик управляемых доменов.</span><span class="sxs-lookup"><span data-stu-id="fe54a-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="fe54a-110">Эта конфигурация создает топологию сетевой сети, которая поддерживает репликацию каталогов.</span><span class="sxs-lookup"><span data-stu-id="fe54a-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="fe54a-111">Виртуальная сеть может поддерживать несколько наборов реплик при условии, что каждый набор реплик находится в другой виртуальной подсети.</span><span class="sxs-lookup"><span data-stu-id="fe54a-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="fe54a-112">Дополнительные сведения о наборе реплик см. в [материале "Реплика концепций".](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="fe54a-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
