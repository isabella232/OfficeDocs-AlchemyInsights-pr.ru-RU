---
title: Назначение групп для роли Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875407"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="1bda8-102">Назначение групп для роли Azure AD</span><span class="sxs-lookup"><span data-stu-id="1bda8-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="1bda8-103">Чтобы назначить группу Azure AD с главным источником в Azure AD для роли Azure AD, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="1bda8-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="1bda8-104">Создание группы. Чтобы создать группу:</span><span class="sxs-lookup"><span data-stu-id="1bda8-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="1bda8-105">а.</span><span class="sxs-lookup"><span data-stu-id="1bda8-105">a.</span></span> <span data-ttu-id="1bda8-106">Войдите в Центр администрирования Azure AD с разрешениями **администратора привилегированных ролей** или **глобального администратора**.</span><span class="sxs-lookup"><span data-stu-id="1bda8-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="1bda8-107">б.</span><span class="sxs-lookup"><span data-stu-id="1bda8-107">b.</span></span> <span data-ttu-id="1bda8-108">Выберите **Azure Active Directory > Группы > Все группы > Создать группу**.</span><span class="sxs-lookup"><span data-stu-id="1bda8-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="1bda8-109">в.</span><span class="sxs-lookup"><span data-stu-id="1bda8-109">c.</span></span> <span data-ttu-id="1bda8-110">Создайте группу.</span><span class="sxs-lookup"><span data-stu-id="1bda8-110">Create the group.</span></span>

2. <span data-ttu-id="1bda8-111">Назначьте группе роль во время создания группы или после ее создания.</span><span class="sxs-lookup"><span data-stu-id="1bda8-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="1bda8-112">а.</span><span class="sxs-lookup"><span data-stu-id="1bda8-112">a.</span></span> <span data-ttu-id="1bda8-113">Чтобы назначить роль во время создания группы, включите переключатель **Возможность назначения группе ролей Azure AD** и создайте группу.</span><span class="sxs-lookup"><span data-stu-id="1bda8-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="1bda8-114">б.</span><span class="sxs-lookup"><span data-stu-id="1bda8-114">b.</span></span> <span data-ttu-id="1bda8-115">Чтобы назначить роль после создания группы, перейдите на вкладку **Назначенные роли** созданной группы и назначьте ей роль.</span><span class="sxs-lookup"><span data-stu-id="1bda8-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="1bda8-116">**Управление участием в группе, которой назначена роль Azure AD**</span><span class="sxs-lookup"><span data-stu-id="1bda8-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="1bda8-117">Чтобы не допустить повышения привилегий, по умолчанию только администраторы привилегированных ролей и глобальные администраторы могут изменять участников группы, которой назначена роль.</span><span class="sxs-lookup"><span data-stu-id="1bda8-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="1bda8-118">Тем не менее, они могут назначить владельца для такой группы и делегировать эту задачу.</span><span class="sxs-lookup"><span data-stu-id="1bda8-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="1bda8-119">Дополнительные сведения о назначении ролей Azure AD облачным группам в статье [Назначение ролей AD облачной группе](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="1bda8-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="1bda8-120">Дополнительные сведения об устранении неполадок с ролями, назначенными облачным группам, см. в статье [Устранение неполадок с ролями, назначенными облачным группам](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="1bda8-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





