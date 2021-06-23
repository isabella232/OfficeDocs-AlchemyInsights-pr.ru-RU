---
title: Включение проверки подлинности SMTP и устранение неполадок
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077664"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="ffdad-102">Включение проверки подлинности SMTP и устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="ffdad-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="ffdad-103">Если вы хотите включить проверку подлинности SMTP для почтового ящика или у вас возникает ошибка "Клиент не прошел проверку подлинности", "Неудачная проверка подлинности" или "SmtpClientAuthentication" с кодом 5.7.57, 5.7.3 или 5.7.139 при попытке ретрансляции электронной почты путем проверки подлинности устройства или приложения в Microsoft 365, выполните три действия для устранения проблемы:</span><span class="sxs-lookup"><span data-stu-id="ffdad-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="ffdad-104">Отключите [параметры безопасности по умолчанию Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) путем переключения настройки **Включение параметров безопасности по умолчанию** в положение **Нет**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="ffdad-105">а.</span><span class="sxs-lookup"><span data-stu-id="ffdad-105">a.</span></span> <span data-ttu-id="ffdad-106">Войдите на портал Azure от имени администратора безопасности, администратора условного доступа или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="ffdad-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="ffdad-107">б.</span><span class="sxs-lookup"><span data-stu-id="ffdad-107">b.</span></span> <span data-ttu-id="ffdad-108">Перейдите в раздел Azure Active Directory > **Свойства**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="ffdad-109">в.</span><span class="sxs-lookup"><span data-stu-id="ffdad-109">c.</span></span> <span data-ttu-id="ffdad-110">Выберите **Управление параметрами безопасности по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="ffdad-111">г.</span><span class="sxs-lookup"><span data-stu-id="ffdad-111">d.</span></span> <span data-ttu-id="ffdad-112">Присвойте настройке **Включение параметров безопасности по умолчанию** значение **Нет**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="ffdad-113">д.</span><span class="sxs-lookup"><span data-stu-id="ffdad-113">e.</span></span> <span data-ttu-id="ffdad-114">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-114">Select **Save**.</span></span>

2. <span data-ttu-id="ffdad-115">[Включите отправку SMTP клиента](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) в лицензированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ffdad-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="ffdad-116">а.</span><span class="sxs-lookup"><span data-stu-id="ffdad-116">a.</span></span> <span data-ttu-id="ffdad-117">В Центре администрирования Microsoft 365 перейдите в раздел **Активные пользователи** и выберите пользователя.</span><span class="sxs-lookup"><span data-stu-id="ffdad-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="ffdad-118">б.</span><span class="sxs-lookup"><span data-stu-id="ffdad-118">b.</span></span> <span data-ttu-id="ffdad-119">Перейдите на вкладку "Почта" и в разделе **Почтовые приложения** выберите **Управление приложениями электронной почты**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="ffdad-120">г.</span><span class="sxs-lookup"><span data-stu-id="ffdad-120">d.</span></span> <span data-ttu-id="ffdad-121">Установите флажок **SMTP с проверкой подлинности** (параметр включен).</span><span class="sxs-lookup"><span data-stu-id="ffdad-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="ffdad-122">д.</span><span class="sxs-lookup"><span data-stu-id="ffdad-122">e.</span></span> <span data-ttu-id="ffdad-123">Нажмите **Сохранить изменения**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="ffdad-124">[Отключите многофакторную проверку подлинности (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) в лицензированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ffdad-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="ffdad-125">а.</span><span class="sxs-lookup"><span data-stu-id="ffdad-125">a.</span></span> <span data-ttu-id="ffdad-126">Перейдите в Центр администрирования Microsoft 365 и в меню навигации слева выберите **Пользователи** > **Активные пользователи**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="ffdad-127">б.</span><span class="sxs-lookup"><span data-stu-id="ffdad-127">b.</span></span> <span data-ttu-id="ffdad-128">Выберите **Многофакторная проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="ffdad-129">в.</span><span class="sxs-lookup"><span data-stu-id="ffdad-129">c.</span></span> <span data-ttu-id="ffdad-130">Выберите пользователя и отключите **многофакторную проверку подлинности**.</span><span class="sxs-lookup"><span data-stu-id="ffdad-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
