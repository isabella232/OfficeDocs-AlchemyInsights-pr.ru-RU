---
title: Monitor Intune Conditional Access
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417319"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="f9375-102">Monitor Intune Conditional Access</span><span class="sxs-lookup"><span data-stu-id="f9375-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="f9375-103">Пользователи с условным доступом получат уведомление по электронной почте, если они не соответствуют требованиям к доступу вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f9375-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f9375-104">Для решения рекомендуется одно или несколько следующих решений:</span><span class="sxs-lookup"><span data-stu-id="f9375-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="f9375-105">Если предполагается, что устройство зарегистрируется, советуйте пользователю перейти в приложение Портал компании и убедиться, что оно отображается на портале компании.</span><span class="sxs-lookup"><span data-stu-id="f9375-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f9375-106">Если этого не сделать, пользователь должен записать устройство.</span><span class="sxs-lookup"><span data-stu-id="f9375-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="f9375-107">На портале Azure перейдите к **соблюдению требований к устройству Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="f9375-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="f9375-108">Чтобы просмотреть отчет о соответствии устройств, чтобы убедиться, что устройство пользователя помечено как совместимый, в **статье Monitor** нажмите **кнопку Соответствие устройству.**</span><span class="sxs-lookup"><span data-stu-id="f9375-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="f9375-109">На портале Azure перейдите к **соблюдению требований к устройству Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="f9375-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="f9375-110">В **статье Управление щелкните** **Политики**.</span><span class="sxs-lookup"><span data-stu-id="f9375-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="f9375-111">В списке политик соответствия требованиям убедитесь, что профиль назначен устройству пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9375-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f9375-112">Если профиль не назначен, intune не сможет подтвердить состояние соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="f9375-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="f9375-113">Изменение назначения условного доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9375-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="f9375-114">На портале Azure перейдите к политикам условного доступа **Intune,** выберите политику из списка и нажмите  >    >  кнопку **Пользователи и группы.**</span><span class="sxs-lookup"><span data-stu-id="f9375-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="f9375-115">Чтобы на кого-то нацелить определенную политику, добавьте их в список **Include.**</span><span class="sxs-lookup"><span data-stu-id="f9375-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="f9375-116">Чтобы исключить человека из политики, добавьте его в список **Исключений.**</span><span class="sxs-lookup"><span data-stu-id="f9375-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="f9375-117">**Полезные ссылки:**</span><span class="sxs-lookup"><span data-stu-id="f9375-117">**Helpful links:**</span></span>

- [<span data-ttu-id="f9375-118">Обзор соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="f9375-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="f9375-119">Устранение неполадок в ЦС</span><span class="sxs-lookup"><span data-stu-id="f9375-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="f9375-120">Политика устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="f9375-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="f9375-121">Мониторинг соответствия устройствам Intune</span><span class="sxs-lookup"><span data-stu-id="f9375-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="f9375-122">Эти действия полезны только для устранения неполадок с функцией Условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9375-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="f9375-123">Кроме того, можно карантить устройство, блокирующее доступ к электронной почте с помощью политики Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9375-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="f9375-124">Дополнительные сведения об управлении устройствами Exchange можно найти [**здесь.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="f9375-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
