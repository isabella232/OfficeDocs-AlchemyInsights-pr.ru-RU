---
title: Условный доступ с помощью Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706034"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="55b9e-102">Условный доступ с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="55b9e-102">Conditional Access with Intune</span></span>

<span data-ttu-id="55b9e-103">Для использования **условного доступа** в Intune необходимо 3 этапа:</span><span class="sxs-lookup"><span data-stu-id="55b9e-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="55b9e-104">Создайте **политику условного доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="55b9e-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="55b9e-105">Например, устройство должно быть совместимо перед доступом к корпоративной почте.</span><span class="sxs-lookup"><span data-stu-id="55b9e-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="55b9e-106">Создайте **политику соответствия требованиям** , чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым.</span><span class="sxs-lookup"><span data-stu-id="55b9e-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="55b9e-107">Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым.</span><span class="sxs-lookup"><span data-stu-id="55b9e-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="55b9e-108">Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей.</span><span class="sxs-lookup"><span data-stu-id="55b9e-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="55b9e-109">Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="55b9e-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="55b9e-110">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="55b9e-110">Read more:</span></span>
  
- [<span data-ttu-id="55b9e-111">Рекомендации по условному доступу</span><span class="sxs-lookup"><span data-stu-id="55b9e-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="55b9e-112">Начало работы с условным доступом</span><span class="sxs-lookup"><span data-stu-id="55b9e-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

