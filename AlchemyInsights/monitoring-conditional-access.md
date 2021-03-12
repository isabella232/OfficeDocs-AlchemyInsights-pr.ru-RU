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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708687"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="4398e-102">Мониторинг условного доступа для Exchange</span><span class="sxs-lookup"><span data-stu-id="4398e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="4398e-103">Пользователи с условным доступом получат уведомление по электронной почте, если они не соответствуют требованиям к доступу вашей организации.</span><span class="sxs-lookup"><span data-stu-id="4398e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="4398e-104">Для решения рекомендуется одно или несколько следующих решений:</span><span class="sxs-lookup"><span data-stu-id="4398e-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="4398e-105">Если предполагается, что устройство зарегистрируется, советуйте пользователю перейти в приложение Портал компании и убедиться, что оно отображается на портале компании.</span><span class="sxs-lookup"><span data-stu-id="4398e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="4398e-106">Если этого не сделать, пользователь должен записать устройство.</span><span class="sxs-lookup"><span data-stu-id="4398e-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="4398e-107">На портале Azure перейдите в службу соответствия требованиям > устройств.</span><span class="sxs-lookup"><span data-stu-id="4398e-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="4398e-108">В статье Monitor нажмите кнопку Соответствие устройству.</span><span class="sxs-lookup"><span data-stu-id="4398e-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="4398e-109">Просмотреть отчет о соответствии устройству, чтобы убедиться, что устройство пользователя помечено как соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="4398e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="4398e-110">На портале Azure перейдите в службу соответствия требованиям > устройств.</span><span class="sxs-lookup"><span data-stu-id="4398e-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="4398e-111">В статье Управление щелкните Политики.</span><span class="sxs-lookup"><span data-stu-id="4398e-111">Under Manage, click Policies.</span></span> <span data-ttu-id="4398e-112">В списке политик соответствия требованиям убедитесь, что профиль назначен устройству пользователя.</span><span class="sxs-lookup"><span data-stu-id="4398e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="4398e-113">Если профиль не назначен, intune не сможет подтвердить состояние соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="4398e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="4398e-114">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="4398e-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="4398e-115">На портале Azure перейдите к политикам условного доступа **Intune.**  >    >  </span><span class="sxs-lookup"><span data-stu-id="4398e-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="4398e-116">Выберите политику из списка.</span><span class="sxs-lookup"><span data-stu-id="4398e-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="4398e-117">Щелкните Пользователи и группы.</span><span class="sxs-lookup"><span data-stu-id="4398e-117">Click Users and groups.</span></span>
4. <span data-ttu-id="4398e-118">Чтобы на кого-то нацелить определенную политику, добавьте их в список Include.</span><span class="sxs-lookup"><span data-stu-id="4398e-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="4398e-119">Чтобы исключить человека из политики, добавьте его в список Исключений.</span><span class="sxs-lookup"><span data-stu-id="4398e-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="4398e-120">Полезные ссылки:</span><span class="sxs-lookup"><span data-stu-id="4398e-120">Helpful links:</span></span>

[<span data-ttu-id="4398e-121">Обзор соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="4398e-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="4398e-122">Устранение неполадок в ЦС</span><span class="sxs-lookup"><span data-stu-id="4398e-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="4398e-123">Политика устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="4398e-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="4398e-124">Мониторинг соответствия устройствам Intune</span><span class="sxs-lookup"><span data-stu-id="4398e-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="4398e-125">Примечание. Эти действия полезны только для устранения неполадок с функцией Условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4398e-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="4398e-126">Кроме того, можно карантить устройство, блокирующее доступ к электронной почте с помощью политики Exchange.</span><span class="sxs-lookup"><span data-stu-id="4398e-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="4398e-127">Дополнительные сведения об управлении устройствами Exchange можно найти [здесь]. https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="4398e-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
