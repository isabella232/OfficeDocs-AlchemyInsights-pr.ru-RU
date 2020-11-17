---
title: Привилегированная роль управления удостоверениями
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086378"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="8f42e-102">Привилегированная роль управления удостоверениями (PIM)</span><span class="sxs-lookup"><span data-stu-id="8f42e-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="8f42e-103">**После активации роли разрешения не предоставляются**</span><span class="sxs-lookup"><span data-stu-id="8f42e-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="8f42e-104">При активации роли в службе управления правами для привилегированного управления идентификаторами Azure AD Активация может быть непростой для всех порталов, требующих привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="8f42e-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="8f42e-105">Иногда, даже если изменение распространяется, веб-кэширование на портале может привести к тому, что изменения не вступят в силу немедленно.</span><span class="sxs-lookup"><span data-stu-id="8f42e-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="8f42e-106">Если активация задерживается, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="8f42e-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="8f42e-107">Выйдите из Azure Portal и войдите снова.</span><span class="sxs-lookup"><span data-stu-id="8f42e-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="8f42e-108">При активации роли Azure AD или роли ресурса Azure вы увидите этапы активации.</span><span class="sxs-lookup"><span data-stu-id="8f42e-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="8f42e-109">По завершении всех этапов отображается ссылка "выйти".</span><span class="sxs-lookup"><span data-stu-id="8f42e-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="8f42e-110">Эту ссылку можно использовать для выхода. В большинстве случаев задержка активации будет устранена.</span><span class="sxs-lookup"><span data-stu-id="8f42e-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="8f42e-111">В разделе PIM убедитесь, что вы перечислены в качестве члена роли.</span><span class="sxs-lookup"><span data-stu-id="8f42e-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="8f42e-112">Если вы активируете роль администратора Exchange, не забудьте выйти и войти снова.</span><span class="sxs-lookup"><span data-stu-id="8f42e-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="8f42e-113">Если проблема повторяется, откройте билет поддержки и повысьте это как проблему.</span><span class="sxs-lookup"><span data-stu-id="8f42e-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="8f42e-114">Если вы используете роль администратора Exchange для доступа к центру безопасности и соответствия требованиям, обратитесь к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="8f42e-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="8f42e-115">Если вы активируете роль для доступа к центру безопасности и соответствия требованиям или активируете роль администратора SharePoint, вы будете испытывать некоторую задержку при активации от нескольких минут до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="8f42e-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="8f42e-116">Это известная проблема, и мы активно работаем с этими командами, чтобы решить эту проблему как можно скорее.</span><span class="sxs-lookup"><span data-stu-id="8f42e-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="8f42e-117">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="8f42e-117">For more information, see:</span></span>

- [<span data-ttu-id="8f42e-118">Активация моих ролей Azure AD в PIM</span><span class="sxs-lookup"><span data-stu-id="8f42e-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="8f42e-119">Активация ролей ресурсов Azure в PIM</span><span class="sxs-lookup"><span data-stu-id="8f42e-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="8f42e-120">**Разрешения не удаляются после отключения роли или истечения срока активации роли**</span><span class="sxs-lookup"><span data-stu-id="8f42e-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="8f42e-121">При отключении роли в службе управления правами для привилегированного пользователя Azure AD или при истечении периода активации для роли может возникнуть задержка, в течение которого вы продолжаете доступ.</span><span class="sxs-lookup"><span data-stu-id="8f42e-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="8f42e-122">Если отключение отложено, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="8f42e-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="8f42e-123">Если вы деактивируйте роль администратора Exchange или истечет срок активации роли, а вы заметили серьезную задержку перед удалением разрешений, откройте билет поддержки и сообщите специалисту службы поддержки о том, как создать билет с помощью группы управления привилегированным доступом (PAM) в Office.</span><span class="sxs-lookup"><span data-stu-id="8f42e-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="8f42e-124">Если период активации истек, но сеанс браузера по-прежнему открыт, закройте браузер.</span><span class="sxs-lookup"><span data-stu-id="8f42e-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="8f42e-125">Вы можете продолжать использовать эту роль до закрытия этого сеанса.</span><span class="sxs-lookup"><span data-stu-id="8f42e-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="8f42e-126">Это известная проблема, и мы рассматриваете возможные исправления, чтобы отменять каждый сеанс после истечения срока активации.</span><span class="sxs-lookup"><span data-stu-id="8f42e-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="8f42e-127">Если задержка отличается от этих двух сценариев, откройте билет поддержки.</span><span class="sxs-lookup"><span data-stu-id="8f42e-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
