---
title: Ошибка "Отказано в доступе" для нескольких пользователей при добавлении надстроек в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397749"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="21cc9-102">Ошибка "Отказано в доступе" для нескольких пользователей при добавлении надстроек в Outlook</span><span class="sxs-lookup"><span data-stu-id="21cc9-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="21cc9-p101">Вы можете указать, каким администраторам в вашей организации разрешается устанавливать надстройки для Outlook и управлять ими. Кроме того, можно указать, каким пользователям в организации будет разрешено устанавливать надстройки и управлять ими для собственных нужд.</span><span class="sxs-lookup"><span data-stu-id="21cc9-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="21cc9-105">Подробные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="21cc9-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="21cc9-106">Чтобы убедиться в том, что вы назначили разрешения для пользователя, замените <Role Name> на название проверяемой роли и выполните следующую команду в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="21cc9-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="21cc9-107">Get-ManagementRoleAssignment -Роль "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="21cc9-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="21cc9-108">В этом примере показано, как проверить, кому назначены разрешения на установку в организации надстроек из Магазина Office.</span><span class="sxs-lookup"><span data-stu-id="21cc9-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="21cc9-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="21cc9-109">PowerShell</span></span>

<span data-ttu-id="21cc9-110">-Роль "Приложения Org Marketplace" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="21cc9-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="21cc9-111">В результатах Get-ManagementRoleAssignment просмотрите записи в столбце "Действующие пользователи".</span><span class="sxs-lookup"><span data-stu-id="21cc9-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="21cc9-112">Дополнительные сведения о синтаксисе и параметрах см. в разделе [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="21cc9-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 