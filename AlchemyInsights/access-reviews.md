---
title: Проверки доступа
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013977"
---
# <a name="access-reviews"></a><span data-ttu-id="03620-102">Проверки доступа</span><span class="sxs-lookup"><span data-stu-id="03620-102">Access reviews</span></span>

1. <span data-ttu-id="03620-103">**Включить проверки доступа:** вы можете включить проверки при создании нового пакета доступа или редактировании существующего пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="03620-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="03620-104">В этой статье описывается, как включить проверки доступа к пакетам доступа, чтобы просмотреть пакеты доступа в службе управления правами [Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create)</span><span class="sxs-lookup"><span data-stu-id="03620-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="03620-105">**Проверка Access:** управление правами Azure AD упрощает управление доступом к группам, приложениям и сайтам SharePoint предприятиями.</span><span class="sxs-lookup"><span data-stu-id="03620-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="03620-106">Обзор доступа к пакету доступа в управлении правами [Azure AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) описывает, как выполнять проверки доступа для других пользователей, назначенных пакету доступа в качестве назначенного рецензента.</span><span class="sxs-lookup"><span data-stu-id="03620-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="03620-107">**Просмотрите access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span><span class="sxs-lookup"><span data-stu-id="03620-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="03620-108">В большинстве случаев конечные пользователи находят отзыв в ожидании ответа на панели **доступа.**</span><span class="sxs-lookup"><span data-stu-id="03620-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="03620-109">Это применимо только к отзывам групп и приложений, а не к ролям.</span><span class="sxs-lookup"><span data-stu-id="03620-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="03620-110">Для всех проверок доступа к ролям конечные пользователи должны перейти к azure AD Privileged Identity Management (PIM), чтобы завершить проверку.</span><span class="sxs-lookup"><span data-stu-id="03620-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="03620-111">Во время logon to the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="03620-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="03620-112">Перейдите в Azure AD PIM.</span><span class="sxs-lookup"><span data-stu-id="03620-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="03620-113">В левой области навигации выберите доступ **для**  >  **проверки задач.**</span><span class="sxs-lookup"><span data-stu-id="03620-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="03620-114">Дополнительные сведения см. в следующих статьях.</span><span class="sxs-lookup"><span data-stu-id="03620-114">For more information, see:</span></span>

- [<span data-ttu-id="03620-115">Проверка доступа к ролям каталога Azure AD в PIM </span><span class="sxs-lookup"><span data-stu-id="03620-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="03620-116">Проверка доступа к ролям ресурсов Azure в PIM</span><span class="sxs-lookup"><span data-stu-id="03620-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)