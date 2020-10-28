---
title: Доступ к подписке
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773781"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="9996c-102">Не удается выполнить вход в Azure из-за проблем с браузером (зависание браузера, не загружается, не загружается и т. д.).</span><span class="sxs-lookup"><span data-stu-id="9996c-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="9996c-103">Возможно, вы повлияли на отключение.</span><span class="sxs-lookup"><span data-stu-id="9996c-103">You might be impacted by an outage.</span></span> <span data-ttu-id="9996c-104">Проверьте, существует ли непрерывный сбой: [состояние работоспособности Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="9996c-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="9996c-105">Выйдите из всех активных сеансов Azure.</span><span class="sxs-lookup"><span data-stu-id="9996c-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="9996c-106">Запустите собственный или инкогнито режим веб-браузера.</span><span class="sxs-lookup"><span data-stu-id="9996c-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="9996c-107">Вы также можете попробовать обновить браузер, использовать другой браузер, удалить файлы cookie кэша, если они не работают.</span><span class="sxs-lookup"><span data-stu-id="9996c-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="9996c-108">Дополнительные сведения: [Устранение проблем с входом](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="9996c-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="9996c-109">**Не удается получить доступ к подпискам**</span><span class="sxs-lookup"><span data-stu-id="9996c-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="9996c-110">На [портале Azure](https://portal.azure.com/)убедитесь, что выбран правильный каталог Azure из учетной записи в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="9996c-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="9996c-111">В [центре учетных записей Azure](https://account.windowsazure.com/Subscriptions)убедитесь, что используемая учетная запись является администратором учетной записи.</span><span class="sxs-lookup"><span data-stu-id="9996c-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="9996c-112">Дополнительные сведения: [Устранение неполадок подписки не найдены](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="9996c-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="9996c-113">**Не удается получить доступ к журналу выставления счетов**</span><span class="sxs-lookup"><span data-stu-id="9996c-113">**Unable to access billing history**</span></span>

<span data-ttu-id="9996c-114">Администратору учетной записи необходимо убедиться, что пользователь, обращающийся к сведениям для выставления счетов, добавлен в Azure Active Directory в качестве пользователя-гостя: [Добавление или удаление нового пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9996c-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9996c-115">Затем пользователю должна быть назначена роль глобального администратора: [назначение роли пользователям](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9996c-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9996c-116">Опубликовать это, пользователю может быть предоставлен доступ к оплате с помощью политик RBAC: [предоставление доступа к выставлению счетов](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9996c-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9996c-117">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="9996c-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="9996c-118">Не удается выполнить вход для управления моей подпиской Azure</span><span class="sxs-lookup"><span data-stu-id="9996c-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)