---
title: Устранение неполадок SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428833"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="83489-102">Устранение неполадок SSPR</span><span class="sxs-lookup"><span data-stu-id="83489-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="83489-103">**У меня возникли проблемы с настройкой сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="83489-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="83489-104">Если вы администратор и ищете, как включить сброс пароля самообслуживаемых, см. в учебнике включить [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), чтобы настроить сброс пароля для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="83489-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="83489-105">Кроме того, может потребоваться просмотреть [требования к лицензированию.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="83489-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="83489-106">В организации должна быть назначена по крайней мере одна лицензия.</span><span class="sxs-lookup"><span data-stu-id="83489-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="83489-107">**Только пользователи облачных** вычислений . Любой Office 365 (O365) платный SKU или Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="83489-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="83489-108">**Облачные и/или** локально пользователи - Azure AD Premium P1 или P2, Корпоративная мобильность и безопасность (EMS) или Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="83489-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="83489-109">Дополнительные вопросы об сбросе паролей самообслуживаем читайте [в нашем faQ.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="83489-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="83489-110">**Я получаю сообщение об ошибке**</span><span class="sxs-lookup"><span data-stu-id="83489-110">**I'm getting an error message**</span></span>

<span data-ttu-id="83489-111">Просмотрите эту статью, чтобы найти распространенные ошибки и их решения: сброс пароля [самообслуживления](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="83489-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="83489-112">**У меня возникли проблемы с политикой сброса паролей**</span><span class="sxs-lookup"><span data-stu-id="83489-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="83489-113">Если политика сброса паролей ведет себя не так, как ожидалось, или у вас есть вопросы по политикам сброса паролей, просмотрите эту статью: политики паролей и ограничения в [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="83489-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="83489-114">Политики сброса паролей не применяются к администраторам.</span><span class="sxs-lookup"><span data-stu-id="83489-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="83489-115">Корпорация Майкрософт применяет сильную политику сброса паролей с двумя воротами по умолчанию для любой роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="83489-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="83489-116">Убедитесь, что вы тестируете с пользователем, который не является администратором.</span><span class="sxs-lookup"><span data-stu-id="83489-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="83489-117">Дополнительные сведения о политике сброса администратора см. в этой [статье.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="83489-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="83489-118">**Я не хочу, чтобы мои пользователи регистрируют дополнительные сведения о безопасности для сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="83489-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="83489-119">Вы можете предварительно заполнить данные (атрибуты электронной почты и телефона) для пользователей с помощью API, PowerShell или Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="83489-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="83489-120">Чтобы узнать, как читать:</span><span class="sxs-lookup"><span data-stu-id="83489-120">To learn how read:</span></span>

- [<span data-ttu-id="83489-121">Развертывание сброса пароля без необходимости регистрации пользователей</span><span class="sxs-lookup"><span data-stu-id="83489-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="83489-122">Какие данные используются при сбросе пароля</span><span class="sxs-lookup"><span data-stu-id="83489-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="83489-123">**Я хочу, чтобы мои пользователи зарегистрировали свои дополнительные сведения о безопасности для сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="83489-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="83489-124">Чтобы пользователи зарегистрировали свои сведения о безопасности для сброса пароля самообслуживки, направив их на [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="83489-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="83489-125">После заполнения данных пользователем (пользователем или администратором) направите aka.ms/sspr, чтобы пользователи могли сбросить собственные пароли. [](https://passwordreset.microsoftonline.com/)</span><span class="sxs-lookup"><span data-stu-id="83489-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="83489-126">Если пользователи по-прежнему испытывают проблемы, они, скорее всего, **федерария** или **пароль hash synched** пользователей.</span><span class="sxs-lookup"><span data-stu-id="83489-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="83489-127">Это означает, что существует проблема со службой записи паролей.</span><span class="sxs-lookup"><span data-stu-id="83489-127">This means there is likely a problem with the Password Writeback service.</span></span>