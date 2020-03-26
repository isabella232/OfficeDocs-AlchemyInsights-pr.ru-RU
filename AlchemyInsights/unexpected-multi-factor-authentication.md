---
title: Внеплановая многофакторная проверка подлинности
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946733"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="33a51-102">Внеплановая многофакторная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="33a51-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="33a51-103">Если ваш клиент был создан позднее 21 октября 2019 г. и вам неожиданно предлагают пройти MFA, скорее всего, в вашем клиенте включены [параметры безопасности по умолчанию](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="33a51-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="33a51-104">Для управления параметрами безопасности по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="33a51-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="33a51-105">Войдите в [Центр администрирования](https://go.microsoft.com/fwlink/p/?linkid=834822) с учетными данными глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="33a51-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="33a51-106">Перейдите в раздел [Свойства Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="33a51-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="33a51-107">В нижней части страницы щелкните **Управление параметрами безопасности по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="33a51-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="33a51-108">Нажмите кнопку **Да**, чтобы включить параметры безопасности по умолчанию, или **Нет**, чтобы их отключить.</span><span class="sxs-lookup"><span data-stu-id="33a51-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
