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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366441"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="c5075-102">Мониторинг условного доступа для Exchange</span><span class="sxs-lookup"><span data-stu-id="c5075-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="c5075-103">Пользователи, которым назначен условный доступ, получат уведомление по электронной почте, если они не отвечают требованиям вашей организации.</span><span class="sxs-lookup"><span data-stu-id="c5075-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="c5075-104">Для решения этой проблемы рекомендуется одно или несколько из следующих решений:</span><span class="sxs-lookup"><span data-stu-id="c5075-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="c5075-105">Если устройство предположительно будет зарегистрировано, посоветуйте пользователю перейти на приложение "Корпоративный портал" и убедиться, что оно отображается на портале компании.</span><span class="sxs-lookup"><span data-stu-id="c5075-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="c5075-106">В противном случае пользователь должен зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="c5075-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="c5075-107">На портале Azure перейдите в Intune > соответствие требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="c5075-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c5075-108">В разделе Мониторинг выберите пункт соответствие устройств.</span><span class="sxs-lookup"><span data-stu-id="c5075-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="c5075-109">Просмотрите отчет о соответствии устройств, чтобы убедиться, что устройство пользователя помечено как соответствующее требованиям.</span><span class="sxs-lookup"><span data-stu-id="c5075-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="c5075-110">На портале Azure перейдите в Intune > соответствие требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="c5075-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c5075-111">В разделе Управление выберите пункт политики.</span><span class="sxs-lookup"><span data-stu-id="c5075-111">Under Manage, click Policies.</span></span> <span data-ttu-id="c5075-112">В списке политик соответствия убедитесь, что для устройства пользователя назначен профиль.</span><span class="sxs-lookup"><span data-stu-id="c5075-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="c5075-113">Если профили не назначены, Intune не сможет подтвердить состояние соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="c5075-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="c5075-114">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5075-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="c5075-115">На портале Azure перейдите в **Intune**раздел  >  **политики условного доступа**Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="c5075-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="c5075-116">Выберите политику из списка.</span><span class="sxs-lookup"><span data-stu-id="c5075-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="c5075-117">Щелкните Пользователи и группы.</span><span class="sxs-lookup"><span data-stu-id="c5075-117">Click Users and groups.</span></span>
4. <span data-ttu-id="c5075-118">Чтобы назначить определенную политику другому пользователю, добавьте ее в список включаемых файлов.</span><span class="sxs-lookup"><span data-stu-id="c5075-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="c5075-119">Чтобы убедиться, что пользователь отсутствует в политике, добавьте его в список исключений.</span><span class="sxs-lookup"><span data-stu-id="c5075-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="c5075-120">Полезные ссылки:</span><span class="sxs-lookup"><span data-stu-id="c5075-120">Helpful links:</span></span>

[<span data-ttu-id="c5075-121">Обзор соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="c5075-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c5075-122">Устранение неполадок ЦС</span><span class="sxs-lookup"><span data-stu-id="c5075-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c5075-123">Политика устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="c5075-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="c5075-124">Мониторинг соответствия требованиям к устройствам Intune</span><span class="sxs-lookup"><span data-stu-id="c5075-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="c5075-125">Примечание: эти действия полезны только при устранении неполадок с условным доступом к функциям Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5075-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="c5075-126">Кроме того, можно помещать блокировку устройства на почтовые устройства с помощью политики Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5075-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="c5075-127">Дополнительные сведения об управлении устройствами Exchange можно найти [здесь](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="c5075-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
