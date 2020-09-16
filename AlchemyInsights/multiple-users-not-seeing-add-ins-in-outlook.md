---
title: Многие пользователи не видят надстройки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729884"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="43074-102">Многие пользователи не видят надстройки в Outlook</span><span class="sxs-lookup"><span data-stu-id="43074-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="43074-103">Если вы тестируете надстройки Outlook и они не отображаются, в качестве первого действия по устранению неполадок используйте командлет PowerShell **Get-OrganizationConfig**, чтобы запросить параметр _AppsForOfficeEnabled_.</span><span class="sxs-lookup"><span data-stu-id="43074-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="43074-104">Если запрос возвращает значение **False**, настройте для этого параметра значение **True** с помощью командлета **Set-OrganizationConfig**, чтобы надстройки отображались должным образом.</span><span class="sxs-lookup"><span data-stu-id="43074-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="43074-105">Не рекомендуется устанавливать для параметра _AppsForOfficeEnabled_ значение **False**.</span><span class="sxs-lookup"><span data-stu-id="43074-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="43074-106">Значение **False** переопределяет все указанные выше параметры административных и пользовательских ролей и блокирует активацию всех новых приложений любым пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="43074-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="43074-107">Дополнительные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="43074-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>