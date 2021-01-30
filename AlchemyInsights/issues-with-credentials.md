---
title: Проблемы с учетными данными
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052955"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="edf0e-102">Проблемы с учетными данными</span><span class="sxs-lookup"><span data-stu-id="edf0e-102">Issues with credentials</span></span>

<span data-ttu-id="edf0e-103">Платформа удостоверений Майкрософт и поток учетных данных клиента [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) описывают, как напрямую программировать поток предоставления учетных данных клиента OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="edf0e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="edf0e-104">**Как управлять паролем или учетными данными сертификата приложения?**</span><span class="sxs-lookup"><span data-stu-id="edf0e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="edf0e-105">В Azure CLI можно использовать учетные данные приложения [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) для удаления, списка или сброса пароля приложения или учетных данных сертификата.</span><span class="sxs-lookup"><span data-stu-id="edf0e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="edf0e-106">**Как пользователи сбрасывают свои пароли?**</span><span class="sxs-lookup"><span data-stu-id="edf0e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="edf0e-107">Пользователям необходимо [зарегистрироваться для самостоятельного сброса](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) пароля, прежде чем они смогут сбросить свои пароли.</span><span class="sxs-lookup"><span data-stu-id="edf0e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="edf0e-108">После регистрации пользователь может следовать инструкциям в этой статье, чтобы сбросить свой пароль: сбросить рабочий или [учебный пароль.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="edf0e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="edf0e-109">**Как пользователи могут изменить свои пароли?**</span><span class="sxs-lookup"><span data-stu-id="edf0e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="edf0e-110">Чтобы изменить пароль, выполните действия, которые необходимо в этой [статье: изменение пароля.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="edf0e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="edf0e-111">Они также могут [управлять паролями приложений для двухшаговой проверки.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="edf0e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="edf0e-112">**Пользователь получает сообщение об ошибке при изменении или сбросе пароля**</span><span class="sxs-lookup"><span data-stu-id="edf0e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="edf0e-113">Эта ссылка предоставляет сведения о распространенных проблемах, которые могут возникнуть при попытке пользователя сбросить пароль: распространенные проблемы и [их решения](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="edf0e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="edf0e-114">**У меня возникла проблема с сбросом пароля пользователя**</span><span class="sxs-lookup"><span data-stu-id="edf0e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="edf0e-115">Убедитесь, что вы уполномочены сбросить пароли.</span><span class="sxs-lookup"><span data-stu-id="edf0e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="edf0e-116">*Сбрасывать пароли пользователей могут только глобальные администраторы, администраторы паролей и администраторы пользователей.*</span><span class="sxs-lookup"><span data-stu-id="edf0e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="edf0e-117">Глобальные администраторы также могут сбрасывать пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="edf0e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="edf0e-118">Убедитесь, что вы понимаете требования к лицензированию:</span><span class="sxs-lookup"><span data-stu-id="edf0e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="edf0e-119">В вашей организации должна быть хотя бы одна лицензия:</span><span class="sxs-lookup"><span data-stu-id="edf0e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="edf0e-120">**Только облачные пользователи:** любой платный SKU Office 365 (O365) или Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="edf0e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="edf0e-121">**Облачные и/или** локально пользователи — Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="edf0e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="edf0e-122">Дополнительные информацию о требованиях к лицензированию см. в требованиях лицензирования для самостоятельного сброса [паролей Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="edf0e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="edf0e-123">Чтобы сбросить пароль пользователя, найдите его в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="edf0e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="edf0e-124">Затем в обзорной blade для этого пользователя нажмите кнопку "сбросить пароль".</span><span class="sxs-lookup"><span data-stu-id="edf0e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="edf0e-125">**Кнопка сброса пароля затеняется**</span><span class="sxs-lookup"><span data-stu-id="edf0e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="edf0e-126">Сброс паролей этого  пользователя не разрешен.</span><span class="sxs-lookup"><span data-stu-id="edf0e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="edf0e-127">*Сбрасывать пароли пользователей могут только глобальные администраторы, администраторы паролей и администраторы пользователей.*</span><span class="sxs-lookup"><span data-stu-id="edf0e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="edf0e-128">Глобальные администраторы также могут сбрасывать пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="edf0e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="edf0e-129">**Я не вижу blade сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="edf0e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="edf0e-130">Сброс паролей не разрешен.</span><span class="sxs-lookup"><span data-stu-id="edf0e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="edf0e-131">*Сбрасывать пароли пользователей могут только глобальные администраторы, администраторы паролей и администраторы пользователей.*</span><span class="sxs-lookup"><span data-stu-id="edf0e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="edf0e-132">Глобальные администраторы также могут сбрасывать пароли других привилегированных администраторов.</span><span class="sxs-lookup"><span data-stu-id="edf0e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="edf0e-133">**Я не вижу в локальной интеграции blade при сбросе пароля**</span><span class="sxs-lookup"><span data-stu-id="edf0e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="edf0e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span><span class="sxs-lookup"><span data-stu-id="edf0e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="edf0e-135">Эта blade не будет отсвеяна, если:</span><span class="sxs-lookup"><span data-stu-id="edf0e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="edf0e-136">Вы не используете для записи пароля</span><span class="sxs-lookup"><span data-stu-id="edf0e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="edf0e-137">Возникла проблема с установкой и подключением для записи паролей</span><span class="sxs-lookup"><span data-stu-id="edf0e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="edf0e-138">Возникла проблема с установкой и подключением Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="edf0e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="edf0e-139">Дополнительные действия по устранению неполадок, которые необходимо предпринять при записи пароля, см. в этой [теме.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="edf0e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="edf0e-140">**Не знаю, как сбросить пароль пользователя**</span><span class="sxs-lookup"><span data-stu-id="edf0e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="edf0e-141">Во sign in to the Azure portal as an appropriate admin.</span><span class="sxs-lookup"><span data-stu-id="edf0e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="edf0e-142">Перейдите в blade **"Пользователи и группы"** и выберите **"Все пользователи".**</span><span class="sxs-lookup"><span data-stu-id="edf0e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="edf0e-143">Выберите пользователя в списке.</span><span class="sxs-lookup"><span data-stu-id="edf0e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="edf0e-144">Для выбранного пользователя выберите **"Обзор",** а затем на панели команд выберите "Сброс **пароля".**</span><span class="sxs-lookup"><span data-stu-id="edf0e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="edf0e-145">Выберите **кнопку сброса** пароля и следуйте инструкциям на экране.</span><span class="sxs-lookup"><span data-stu-id="edf0e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="edf0e-146">Только сбросы, выполняемые с помощью **портала Azure,** поддерживают возврат паролей.</span><span class="sxs-lookup"><span data-stu-id="edf0e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="edf0e-147">**Я сбрасываю пароль локального пользователя с портала администрирования Office 365 или мобильного приложения Office 365, но пользователь по-прежнему не может войти**</span><span class="sxs-lookup"><span data-stu-id="edf0e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="edf0e-148">На этом портале не поддерживается переописка паролей.</span><span class="sxs-lookup"><span data-stu-id="edf0e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="edf0e-149">Сброс пароля пользователя еще раз на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="edf0e-149">Reset the user's password again in the Azure portal.</span></span>
