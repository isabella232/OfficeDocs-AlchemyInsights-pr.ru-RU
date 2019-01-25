---
title: Мониторинг условного доступа
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485965"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="97db2-102">Мониторинг условного доступа</span><span class="sxs-lookup"><span data-stu-id="97db2-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="97db2-p101">С условным доступом пользователи будут получать по электронной почте уведомление, если они не отвечает требованиям вашей организации клиента. Чтобы решить, мы рекомендуем одно или несколько из следующих решений:</span><span class="sxs-lookup"><span data-stu-id="97db2-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="97db2-p102">Если устройство будет считаться участвуют, оповещение пользователя, чтобы перейти к приложения портала компании и убедитесь, что он отображается на портале компании. Если это не так, пользователь должен подать устройства.</span><span class="sxs-lookup"><span data-stu-id="97db2-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="97db2-p103">На портале Azure перейдите к **Intune \> соответствия устройства**. В разделе **мониторинг** щелкните **соответствия устройства**. Просмотр отчета соответствия устройства для проверки устройством пользователя помечается как совместимые.</span><span class="sxs-lookup"><span data-stu-id="97db2-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="97db2-p104">На портале Azure перейдите к **Intune \> соответствия устройства**. В разделе **Управление**щелкните **политики**. В списке политики соответствия убедитесь, что профиль назначается устройства конечных пользователей. Если профиль не назначено, затем Intune нельзя будет для подтверждения соответствия состояние устройства.</span><span class="sxs-lookup"><span data-stu-id="97db2-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="97db2-114">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="97db2-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="97db2-115">На портале Azure перейдите к **Intune \> условного доступа \> политики**</span><span class="sxs-lookup"><span data-stu-id="97db2-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="97db2-116">Выберите соответствующую политику в списке</span><span class="sxs-lookup"><span data-stu-id="97db2-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="97db2-117">Щелкните **пользователи и группы**</span><span class="sxs-lookup"><span data-stu-id="97db2-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="97db2-p105">Для некоторых политику на другого пользователя, добавьте их в список **включений** . Чтобы убедиться, что пользователь задан из политики, добавьте их в список **исключений** .</span><span class="sxs-lookup"><span data-stu-id="97db2-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="97db2-120">Подробнее: [как монитор условного доступа устройств](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="97db2-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

