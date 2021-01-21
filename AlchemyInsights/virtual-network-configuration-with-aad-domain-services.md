---
title: Виртуальная настройка с доменными службами AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884612"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="885d5-102">Виртуальная настройка с доменными службами AAD</span><span class="sxs-lookup"><span data-stu-id="885d5-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="885d5-103">Виртуальная настройка с использованием доменных служб AAD включает следующие действия:</span><span class="sxs-lookup"><span data-stu-id="885d5-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="885d5-104">Проверка работоспособности домена на портале Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="885d5-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="885d5-105">Проверка NSG по поводу правил, которые блокируют порты, необходимые для синхронизации в доменных службах Azure AD, на портале https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="885d5-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="885d5-106">Убедитесь, что виртуальная сеть развернута в том же регионе Azure, что и домен, управляемый доменными службами Azure AD.</span><span class="sxs-lookup"><span data-stu-id="885d5-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="885d5-107">Убедитесь в том, что у вас нет домена с тем же доменным именем, что и в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="885d5-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="885d5-108">Подробнее о рассмотрении проектирования виртуальной сети Azure для поддержки доменных служб AAD см. в статье [Рассмотрение виртуальной сети](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="885d5-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

