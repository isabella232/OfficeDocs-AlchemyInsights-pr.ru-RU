---
title: Проблема с сбросом пароля
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50585654"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="d2e5a-102">Проблемы с сбросом пароля</span><span class="sxs-lookup"><span data-stu-id="d2e5a-102">Problems resetting password</span></span>

<span data-ttu-id="d2e5a-103">Ниже следующую часть проблем, которые могут возникнуть при сбросе пароля, и возможные решения:</span><span class="sxs-lookup"><span data-stu-id="d2e5a-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="d2e5a-104">**У меня возникли проблемы с сбросом пароля, не охваченными в других категориях**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="d2e5a-105">Убедитесь, что вы уполномочены сбросить пароли.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="d2e5a-106">Только администраторы глобальных, паролей и пользователей могут сбросить пароли пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="d2e5a-107">Глобальные администраторы также могут сбросить пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="d2e5a-108">Убедитесь, что вы понимаете требования к лицензированию:</span><span class="sxs-lookup"><span data-stu-id="d2e5a-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="d2e5a-109">В организации должна быть назначена по крайней мере одна лицензия</span><span class="sxs-lookup"><span data-stu-id="d2e5a-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="d2e5a-110">Только пользователи облачных вычислений . Любой Office 365 (O365) платный SKU или Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="d2e5a-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="d2e5a-111">Облачные и/или локально пользователи - Azure AD Premium P1 или P2, Корпоративная мобильность и безопасность (EMS) или Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="d2e5a-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="d2e5a-112">Подробнее о требованиях к лицензированию см. в статье Лицензирование требований к сброшению пароля самообслуживки [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="d2e5a-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="d2e5a-113">**У меня возникают проблемы с тестированием политики сброса паролей, за набором**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="d2e5a-114">Недавно примененные политики могут воспроизводиться во всех центрах обработки данных и конечных точках в течение нескольких минут.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="d2e5a-115">Физическое расстояние от центра обработки данных также влияет на быстрое внесение изменений.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="d2e5a-116">Тестирование с конечным пользователем, а не администратором, и пилот с небольшим набором пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="d2e5a-117">Политики, настроенные только на портале Azure, применяются только к конечным пользователям, а не администраторам.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="d2e5a-118">Корпорация Майкрософт применяет строгую политику сброса паролей по умолчанию для любой роли администратора Azure (пример: глобальный администратор, администратор helpdesk, администратор паролей и т.д.)</span><span class="sxs-lookup"><span data-stu-id="d2e5a-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="d2e5a-119">Дополнительные новости [о политиках для администраторов.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="d2e5a-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="d2e5a-120">**Я хочу развернуть сброс пароля, но не хочу, чтобы пользователи регистрируют дополнительные сведения о безопасности**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="d2e5a-121">Предварительно заполняйте данные для пользователей, чтобы им не нужно было это делать!</span><span class="sxs-lookup"><span data-stu-id="d2e5a-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="d2e5a-122">— В качестве администратора вы можете установить свойства телефона и электронной почты для пользователей перед развертыванием сброса пароля в организации.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="d2e5a-123">Это можно сделать с помощью API, PowerShell или Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="d2e5a-124">Дополнительные сведения здесь:</span><span class="sxs-lookup"><span data-stu-id="d2e5a-124">More information here:</span></span>
- [<span data-ttu-id="d2e5a-125">Развертывание сброса пароля без необходимости регистрации пользователей</span><span class="sxs-lookup"><span data-stu-id="d2e5a-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="d2e5a-126">Какие данные используются при сбросе пароля</span><span class="sxs-lookup"><span data-stu-id="d2e5a-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="d2e5a-127">**Кнопка сброса пароля имеет серый цвет**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="d2e5a-128">Сброс паролей этого пользователя не разрешен.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="d2e5a-129">Только администраторы глобальных, паролей и пользователей могут сбросить пароли пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="d2e5a-130">Глобальные администраторы также могут сбросить пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d2e5a-131">**Я не вижу лопасти сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="d2e5a-132">Сброс паролей не разрешен.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="d2e5a-133">Только администраторы глобальных, паролей и пользователей могут сбросить пароли пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="d2e5a-134">Глобальные администраторы также могут сбросить пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d2e5a-135">**Я не вижу локального лезвия интеграции в сбросе пароля**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="d2e5a-136">Лопасти локальной интеграции появляются только в гибридных средах, что означает, что вы используете списку паролей для обработки паролей локального пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="d2e5a-137">Вы не видите это лезвие, если:</span><span class="sxs-lookup"><span data-stu-id="d2e5a-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="d2e5a-138">Вы не используете возвращение пароля</span><span class="sxs-lookup"><span data-stu-id="d2e5a-138">You are not using password writeback</span></span>
    - <span data-ttu-id="d2e5a-139">Существует проблема с установкой и подключением к записи паролей</span><span class="sxs-lookup"><span data-stu-id="d2e5a-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="d2e5a-140">Существует проблема с установкой и подключением Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d2e5a-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="d2e5a-141">Дополнительные действия по устранению неполадок при списывке паролей см. в разделе [Устранение неполадок.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="d2e5a-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="d2e5a-142">**Я не знаю, как сбросить пароль пользователя**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="d2e5a-143">Во входе на портал Azure в качестве соответствующего администратора.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="d2e5a-144">Перейдите к лезвию Пользователи и группы, выберите **Все пользователи**.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="d2e5a-145">Выберите пользователя из списка.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-145">Select a user from the list.</span></span>
1. <span data-ttu-id="d2e5a-146">Для выбранного пользователя выберите **Обзор,** а затем в панели команд нажмите **кнопку Сброс пароля**.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="d2e5a-147">Следуйте инструкциям на экране.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="d2e5a-148">Только сбросы, выполняемые на портале Azure, поддерживают возврат паролей.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="d2e5a-149">**Сброс пароля локального пользователя с портала Администрирования Office 365 или мобильного приложения Office 365, но пользователь по-прежнему не может войти**</span><span class="sxs-lookup"><span data-stu-id="d2e5a-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="d2e5a-150">Возвращение пароля на этом портале не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e5a-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="d2e5a-151">Сброс пароля пользователя на портале Azure — portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="d2e5a-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

