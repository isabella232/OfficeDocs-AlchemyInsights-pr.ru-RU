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
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931449"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0e13d-102">Условный доступ с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="0e13d-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0e13d-103">Для использования **условного доступа** в Intune необходимо 3 этапа:</span><span class="sxs-lookup"><span data-stu-id="0e13d-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="0e13d-104">Создайте **политику соответствия требованиям** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым.</span><span class="sxs-lookup"><span data-stu-id="0e13d-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="0e13d-105">Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым.</span><span class="sxs-lookup"><span data-stu-id="0e13d-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="0e13d-106">Создайте **политику условного доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="0e13d-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="0e13d-107">[Например,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) устройство должно быть совместимо перед доступом к корпоративной почте.</span><span class="sxs-lookup"><span data-stu-id="0e13d-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="0e13d-108">Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей.</span><span class="sxs-lookup"><span data-stu-id="0e13d-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="0e13d-109">Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e13d-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="0e13d-110">**Полезные ссылки:**</span><span class="sxs-lookup"><span data-stu-id="0e13d-110">**Helpful links:**</span></span>

[<span data-ttu-id="0e13d-111">Обзор соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="0e13d-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0e13d-112">Устранение неполадок ЦС</span><span class="sxs-lookup"><span data-stu-id="0e13d-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0e13d-113">Политика устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="0e13d-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="0e13d-114">Чтобы защитить электронную почту (Exchange Online) от доступа несоответствующих требованиям устройств, необходимо следовать обоим документам:</span><span class="sxs-lookup"><span data-stu-id="0e13d-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="0e13d-115">Защита доступа к электронной почте с устройств, использующих EAS</span><span class="sxs-lookup"><span data-stu-id="0e13d-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="0e13d-116">Защита доступа к электронной почте с устройств с помощью современных клиентов проверки подлинности, таких как Outlook</span><span class="sxs-lookup"><span data-stu-id="0e13d-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)