---
title: Условный доступ с intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704799"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="79dfa-102">Условный доступ с intune</span><span class="sxs-lookup"><span data-stu-id="79dfa-102">Conditional Access with Intune</span></span>

<span data-ttu-id="79dfa-103">Использование  **условного доступа**  с помощью Intune требует 3 действия:</span><span class="sxs-lookup"><span data-stu-id="79dfa-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="79dfa-104">Создайте  **политику соответствия**  требованиям [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows),](https://docs.microsoft.com//intune/compliance-policy-create-windows)чтобы определить параметры, которые необходимо соблюдать, прежде чем устройство будет считаться совместимым.</span><span class="sxs-lookup"><span data-stu-id="79dfa-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="79dfa-105">Например, устройство должно иметь пин-код не менее 6 цифр, прежде чем считать его совместимым.</span><span class="sxs-lookup"><span data-stu-id="79dfa-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="79dfa-106">Создайте **политику условного**  доступа, которая определяет, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="79dfa-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="79dfa-107">[Например, устройство](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  должно быть совместимым перед доступом к корпоративной электронной почте.</span><span class="sxs-lookup"><span data-stu-id="79dfa-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="79dfa-108">Убедитесь, что  политики соответствия **требованиям** и политики условного доступа ориентированы на желаемые группы пользователей.</span><span class="sxs-lookup"><span data-stu-id="79dfa-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="79dfa-109">Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="79dfa-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="79dfa-110">**Полезные ссылки:**</span><span class="sxs-lookup"><span data-stu-id="79dfa-110">**Helpful links:**</span></span>

[<span data-ttu-id="79dfa-111">Обзор соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="79dfa-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="79dfa-112">Устранение неполадок в ЦС</span><span class="sxs-lookup"><span data-stu-id="79dfa-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="79dfa-113">Политика устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="79dfa-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="79dfa-114">Чтобы защитить электронную почту (Exchange online) от доступа с помощью некомплиентных устройств, необходимо следовать обоим документам:</span><span class="sxs-lookup"><span data-stu-id="79dfa-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="79dfa-115">Защита доступа к электронной почте с устройств с помощью EAS</span><span class="sxs-lookup"><span data-stu-id="79dfa-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="79dfa-116">Защита доступа к электронной почте от устройств с помощью современных клиентов проверки подлинности, таких как Outlook</span><span class="sxs-lookup"><span data-stu-id="79dfa-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)