---
title: Условный доступ с помощью Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393554"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0d8f6-102">Условный доступ с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="0d8f6-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0d8f6-103">Для использования **условНого доступа** в Intune необходимо 3 этапа:</span><span class="sxs-lookup"><span data-stu-id="0d8f6-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="0d8f6-104">Создайте **политику условНого доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="0d8f6-105">Например, устройство должно быть совместимо перед доступом к корпоративной почте.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="0d8f6-106">Создайте **политику соответствия требованиям** , чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="0d8f6-107">Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="0d8f6-108">Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="0d8f6-109">Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d8f6-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="0d8f6-110">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="0d8f6-110">Read more:</span></span>
  
- [<span data-ttu-id="0d8f6-111">Рекомендации по условному доступу</span><span class="sxs-lookup"><span data-stu-id="0d8f6-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="0d8f6-112">Начало работы с условным доступом</span><span class="sxs-lookup"><span data-stu-id="0d8f6-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

