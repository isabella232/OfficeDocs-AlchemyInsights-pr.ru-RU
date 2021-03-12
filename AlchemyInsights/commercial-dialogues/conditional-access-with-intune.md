---
title: Использование условного доступа с помощью Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737582"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="b6413-102">Использование условного доступа с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="b6413-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="b6413-103">Использование условного доступа с помощью Intune требует 3 действия:</span><span class="sxs-lookup"><span data-stu-id="b6413-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="b6413-104">Создайте политику соответствия требованиям, чтобы определить параметры, которые должны быть выполнены до того, как устройство будет считаться совместимым. Например, устройство должно иметь пин-код не менее 6 цифр, прежде чем считать его совместимым.</span><span class="sxs-lookup"><span data-stu-id="b6413-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="b6413-105">Создайте политику условного доступа, которая определяет, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам. Например, устройство должно быть совместимым перед доступом к корпоративной электронной почте.</span><span class="sxs-lookup"><span data-stu-id="b6413-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="b6413-106">Убедитесь, что политики соответствия требованиям и политики условного доступа ориентированы на желаемые группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b6413-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b6413-107">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="b6413-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
