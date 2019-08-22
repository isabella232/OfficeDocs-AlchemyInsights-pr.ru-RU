---
title: Мониторинг условного доступа
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538779"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="7bfc3-102">Мониторинг условного доступа для Exchange</span><span class="sxs-lookup"><span data-stu-id="7bfc3-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="7bfc3-103">Пользователи, которым назначен условный доступ, получат уведомление по электронной почте, если они не отвечают требованиям вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7bfc3-104">Для решения этой проблемы рекомендуется одно или несколько из следующих решений:</span><span class="sxs-lookup"><span data-stu-id="7bfc3-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="7bfc3-105">Если устройство предположительно будет зарегистрировано, посоветуйте пользователю перейти на приложение "Корпоративный портал" и убедиться, что оно отображается на портале компании.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7bfc3-106">В противном случае пользователь должен зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="7bfc3-107">На портале Azure перейдите к разделу \*\*соответствие устройства Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7bfc3-108">В разделе **мониторинг** выберите пункт **соответствие устройств**.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="7bfc3-109">Просмотрите отчет о соответствии устройств, чтобы убедиться, что устройство пользователя помечено как соответствующее требованиям.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="7bfc3-110">На портале Azure перейдите к разделу \*\*соответствие устройства Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7bfc3-111">В разделе **Управление**выберите пункт **политики**.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="7bfc3-112">В списке политик соответствия убедитесь, что для устройства пользователя назначен профиль.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7bfc3-113">Если профили не назначены, Intune не сможет подтвердить состояние соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="7bfc3-114">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="7bfc3-115">На портале Azure перейдите в **раздел \> политики условного доступа \> Intune**</span><span class="sxs-lookup"><span data-stu-id="7bfc3-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="7bfc3-116">Выберите политику из списка.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="7bfc3-117">Щелкните **Пользователи и группы** .</span><span class="sxs-lookup"><span data-stu-id="7bfc3-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="7bfc3-118">Чтобы назначить определенную политику другому пользователю, добавьте ее в список **включаемых** файлов.</span><span class="sxs-lookup"><span data-stu-id="7bfc3-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="7bfc3-119">Чтобы убедиться, что пользователь отсутствует в политике, добавьте его в список **исключений** .</span><span class="sxs-lookup"><span data-stu-id="7bfc3-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="7bfc3-120">Дополнительные сведения: [мониторинг устройств с условным доступом](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="7bfc3-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

