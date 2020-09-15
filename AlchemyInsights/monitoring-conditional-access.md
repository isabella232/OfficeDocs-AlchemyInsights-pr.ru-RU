---
title: Мониторинг условного доступа
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702916"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="58a6b-102">Мониторинг условного доступа для Exchange</span><span class="sxs-lookup"><span data-stu-id="58a6b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="58a6b-103">Пользователи, которым назначен условный доступ, получат уведомление по электронной почте, если они не отвечают требованиям вашей организации.</span><span class="sxs-lookup"><span data-stu-id="58a6b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="58a6b-104">Для решения этой проблемы рекомендуется одно или несколько из следующих решений:</span><span class="sxs-lookup"><span data-stu-id="58a6b-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="58a6b-105">Если устройство предположительно будет зарегистрировано, посоветуйте пользователю перейти на приложение "Корпоративный портал" и убедиться, что оно отображается на портале компании.</span><span class="sxs-lookup"><span data-stu-id="58a6b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="58a6b-106">В противном случае пользователь должен зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="58a6b-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="58a6b-107">На портале Azure перейдите к разделу \*\* \> соответствие устройства Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="58a6b-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="58a6b-108">В разделе **мониторинг** выберите пункт **соответствие устройств**.</span><span class="sxs-lookup"><span data-stu-id="58a6b-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="58a6b-109">Просмотрите отчет о соответствии устройств, чтобы убедиться, что устройство пользователя помечено как соответствующее требованиям.</span><span class="sxs-lookup"><span data-stu-id="58a6b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="58a6b-110">На портале Azure перейдите к разделу \*\* \> соответствие устройства Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="58a6b-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="58a6b-111">В разделе **Управление**выберите пункт **политики**.</span><span class="sxs-lookup"><span data-stu-id="58a6b-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="58a6b-112">В списке политик соответствия убедитесь, что для устройства пользователя назначен профиль.</span><span class="sxs-lookup"><span data-stu-id="58a6b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="58a6b-113">Если профили не назначены, Intune не сможет подтвердить состояние соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="58a6b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="58a6b-114">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a6b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="58a6b-115">На портале Azure перейдите в **раздел \> \> политики условного доступа Intune**</span><span class="sxs-lookup"><span data-stu-id="58a6b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="58a6b-116">Выберите политику из списка.</span><span class="sxs-lookup"><span data-stu-id="58a6b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="58a6b-117">Щелкните **Пользователи и группы** .</span><span class="sxs-lookup"><span data-stu-id="58a6b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="58a6b-118">Чтобы назначить определенную политику другому пользователю, добавьте ее в список **включаемых** файлов.</span><span class="sxs-lookup"><span data-stu-id="58a6b-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="58a6b-119">Чтобы убедиться, что пользователь отсутствует в политике, добавьте его в список **исключений** .</span><span class="sxs-lookup"><span data-stu-id="58a6b-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="58a6b-120">Дополнительные сведения: [мониторинг устройств с условным доступом](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="58a6b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

