---
title: Политики условного доступа
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706070"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="80227-102">Политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="80227-102">Conditional Access policies</span></span>

<span data-ttu-id="80227-103">Условный доступ — это возможность Azure AD, позволяющая применять элементы управления при доступе к приложениям в вашей среде в зависимости от конкретных условий и управлять ими централизованно.</span><span class="sxs-lookup"><span data-stu-id="80227-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="80227-104">Узнайте больше об [условном доступе Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="80227-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="80227-105">**Примечание**. Если ваш клиент был создан позднее 21 октября 2019 г. и вам неожиданно предлагают пройти MFA, скорее всего, в вашем клиенте включены [параметры безопасности по умолчанию](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="80227-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="80227-106">**Управление параметрами безопасности по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="80227-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="80227-107">Войдите в [Центр администрирования](https://go.microsoft.com/fwlink/p/?linkid=834822) с учетными данными глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="80227-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="80227-108">Перейдите в раздел [Свойства Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="80227-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="80227-109">В нижней части страницы щелкните **Управление параметрами безопасности по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="80227-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="80227-110">Нажмите **Да**, чтобы включить параметры безопасности по умолчанию, или **Нет**, чтобы их отключить.</span><span class="sxs-lookup"><span data-stu-id="80227-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
