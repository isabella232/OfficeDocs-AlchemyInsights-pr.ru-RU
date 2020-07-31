---
title: Проблемы, возникающие при использовании консоли администрирования Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46523056"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="ac303-102">Проблемы, возникающие при использовании консоли администрирования Intune</span><span class="sxs-lookup"><span data-stu-id="ac303-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="ac303-103">**При переходе на портал администрирования Intune возникает сообщение "Отказано в доступе".**</span><span class="sxs-lookup"><span data-stu-id="ac303-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="ac303-104">Если вы являетесь участником настраиваемой роли Intune, убедитесь, что для вашей учетной записи назначена лицензия на Intune или Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="ac303-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="ac303-105">Если вы используете Configuration Manager для управления устройствами, убедитесь в том, что не являетесь членом коллекции пользователей Intune в Configuration Manager для MDM.</span><span class="sxs-lookup"><span data-stu-id="ac303-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="ac303-106">Убедитесь в том, что вам предоставлены соответствующие разрешения на управление доступом на основе ролей (RBAC) в колонке-ролей Intune.</span><span class="sxs-lookup"><span data-stu-id="ac303-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="ac303-107">Убедитесь в том, что используемая группа не является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="ac303-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="ac303-108">Intune на портале Azure поддерживает только те учетные записи пользователей, которые входят в группы безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ac303-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="ac303-109">Просмотр своих групп на портале Azure > **Intune** > **Группы** или на портале Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="ac303-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="ac303-110">**У пользователя слишком много разрешений для назначенной роли Intune**</span><span class="sxs-lookup"><span data-stu-id="ac303-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="ac303-111">Рекомендуйте пользователю для пересмотра предоставленных разрешений перейти на **Intune** > **Роли Intune** > **Мои разрешения** > **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="ac303-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="ac303-112">**К роли добавлена ограниченная группа, но пользователи в этой роли по-прежнему видят других пользователей или устройства.**</span><span class="sxs-lookup"><span data-stu-id="ac303-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="ac303-113">Ограниченные группы не производят фильтрацию пользователей и устройств.</span><span class="sxs-lookup"><span data-stu-id="ac303-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="ac303-114">Ограниченные группы имеют следующие отличия.</span><span class="sxs-lookup"><span data-stu-id="ac303-114">Scope groups:</span></span>

- <span data-ttu-id="ac303-115">Круг тех, кому пользователи могут назначить политики или приложения, ограничен.</span><span class="sxs-lookup"><span data-stu-id="ac303-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="ac303-116">Запуск удаленных задач на устройствах разрешен только конкретным пользователям.</span><span class="sxs-lookup"><span data-stu-id="ac303-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="ac303-117">Дополнительные сведения об ограниченных группах см. в статье [Управление доступом на основе ролей (RBAC) в Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ac303-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ac303-118">**В роль Intune добавлен пользователь, но он по-прежнему имеет полный доступ к консоли администрирования Intune.**</span><span class="sxs-lookup"><span data-stu-id="ac303-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="ac303-119">На портале Azure перейдите в Intune > **Пользователи** и убедитесь в том, что пользователю на портале Azure не назначены следующие роли:</span><span class="sxs-lookup"><span data-stu-id="ac303-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="ac303-120">глобальный администратор;</span><span class="sxs-lookup"><span data-stu-id="ac303-120">Global administrator</span></span>
- <span data-ttu-id="ac303-121">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="ac303-121">Intune service administrator</span></span>
- <span data-ttu-id="ac303-122">администратор SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ac303-122">SharePoint administrator</span></span>

<span data-ttu-id="ac303-123">Дополнительную информацию см. в статье [Управление доступом на основе ролей (RBAC) в Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ac303-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ac303-124">**Проблемы с доступом**</span><span class="sxs-lookup"><span data-stu-id="ac303-124">**Access Issues**</span></span>

<span data-ttu-id="ac303-125">Дополнительную информацию см. в статье [Проблемы с входом в Office 365, Azure или Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="ac303-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>