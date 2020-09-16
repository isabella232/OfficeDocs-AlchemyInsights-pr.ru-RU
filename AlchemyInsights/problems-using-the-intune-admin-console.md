---
title: Проблемы, возникающие при использовании консоли администрирования Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728300"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="157d6-102">Проблемы, возникающие при использовании консоли администрирования Intune</span><span class="sxs-lookup"><span data-stu-id="157d6-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="157d6-103">**При переходе на портал администрирования Intune возникает сообщение "Отказано в доступе".**</span><span class="sxs-lookup"><span data-stu-id="157d6-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="157d6-104">Если вы являетесь участником настраиваемой роли Intune, убедитесь, что для вашей учетной записи назначена лицензия на Intune или Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="157d6-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="157d6-105">Если вы используете Configuration Manager для управления устройствами, убедитесь в том, что не являетесь членом коллекции пользователей Intune в Configuration Manager для MDM.</span><span class="sxs-lookup"><span data-stu-id="157d6-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="157d6-106">Убедитесь в том, что вам предоставлены соответствующие разрешения на управление доступом на основе ролей (RBAC) в колонке-ролей Intune.</span><span class="sxs-lookup"><span data-stu-id="157d6-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="157d6-107">Убедитесь в том, что используемая группа не является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="157d6-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="157d6-108">Intune на портале Azure поддерживает только те учетные записи пользователей, которые входят в группы безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="157d6-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="157d6-109">Просмотр своих групп на портале Azure > **Intune** > **Группы** или на портале Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="157d6-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="157d6-110">**У пользователя слишком много разрешений для назначенной роли Intune**</span><span class="sxs-lookup"><span data-stu-id="157d6-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="157d6-111">Рекомендуйте пользователю для пересмотра предоставленных разрешений перейти на **Intune** > **Роли Intune** > **Мои разрешения** > **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="157d6-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="157d6-112">**К роли добавлена ограниченная группа, но пользователи в этой роли по-прежнему видят других пользователей или устройства.**</span><span class="sxs-lookup"><span data-stu-id="157d6-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="157d6-113">Ограниченные группы не производят фильтрацию пользователей и устройств.</span><span class="sxs-lookup"><span data-stu-id="157d6-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="157d6-114">Ограниченные группы имеют следующие отличия.</span><span class="sxs-lookup"><span data-stu-id="157d6-114">Scope groups:</span></span>

- <span data-ttu-id="157d6-115">Круг тех, кому пользователи могут назначить политики или приложения, ограничен.</span><span class="sxs-lookup"><span data-stu-id="157d6-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="157d6-116">Запуск удаленных задач на устройствах разрешен только конкретным пользователям.</span><span class="sxs-lookup"><span data-stu-id="157d6-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="157d6-117">Дополнительные сведения об ограниченных группах см. в статье [Управление доступом на основе ролей (RBAC) в Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="157d6-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="157d6-118">**В роль Intune добавлен пользователь, но он по-прежнему имеет полный доступ к консоли администрирования Intune.**</span><span class="sxs-lookup"><span data-stu-id="157d6-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="157d6-119">На портале Azure перейдите в Intune > **Пользователи** и убедитесь в том, что пользователю на портале Azure не назначены следующие роли:</span><span class="sxs-lookup"><span data-stu-id="157d6-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="157d6-120">глобальный администратор;</span><span class="sxs-lookup"><span data-stu-id="157d6-120">Global administrator</span></span>
- <span data-ttu-id="157d6-121">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="157d6-121">Intune service administrator</span></span>
- <span data-ttu-id="157d6-122">администратор SharePoint.</span><span class="sxs-lookup"><span data-stu-id="157d6-122">SharePoint administrator</span></span>

<span data-ttu-id="157d6-123">Дополнительную информацию см. в статье [Управление доступом на основе ролей (RBAC) в Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="157d6-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="157d6-124">**Проблемы с доступом**</span><span class="sxs-lookup"><span data-stu-id="157d6-124">**Access Issues**</span></span>

<span data-ttu-id="157d6-125">Дополнительную информацию см. в статье [Проблемы с входом в Office 365, Azure или Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="157d6-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>