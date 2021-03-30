---
title: Устранение неполадок с гибридным присоединением к Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401920"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="27970-102">Устранение неполадок с гибридным присоединением к Azure AD</span><span class="sxs-lookup"><span data-stu-id="27970-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="27970-103">Настоятельно рекомендуется обеспечить доступ устройства к конечным точкам регистрации устройств в системной учетной записи с помощью [сценария тестирования подключения регистрации устройств](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="27970-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="27970-104">Если вы впервые настраиваете регистрацию устройства, ознакомьтесь с [Введением в управление устройствами в Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), чтобы узнать, как установить контроль Microsoft Azure AD над устройством.</span><span class="sxs-lookup"><span data-stu-id="27970-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="27970-105">Если вы регистрируете устройство непосредственно в Microsoft Azure AD, а затем в Intune, сначала [настройте Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и убедитесь в наличии [лицензий](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="27970-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="27970-106">Убедитесь, что у вас есть права на выполнение операций в Microsoft Azure AD и локальной службе Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27970-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="27970-107">Только глобальный администратор Microsoft Azure AD может управлять параметрами регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="27970-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="27970-108">Кроме того, для настройки автоматической регистрации в локальной службе Active Directory необходимы права администратора Active Directory и AD FS (если применимо).</span><span class="sxs-lookup"><span data-stu-id="27970-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="27970-109">Дополнительные сведения об устранении возможных проблем с гибридным присоединением см. в статье [Устранение неполадок с гибридным присоединением](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Сведения о настройке гибридного присоединения к Azure AD и управлении устройствами с использованием портала Microsoft Azure AD см. в статьях [Настройка устройств с гибридным присоединением к Azure AD (присоединенных к локальному домену)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) и [Управление устройствами с использованием портала Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="27970-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="27970-110">Чтобы устранить распространенные проблемы с гибридным присоединением к Azure Active Directory (AD), см. раздел [Часто задаваемые вопросы о гибридном присоединении к Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="27970-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
