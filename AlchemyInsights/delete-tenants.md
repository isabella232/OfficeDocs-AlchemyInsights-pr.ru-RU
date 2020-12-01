---
title: Удаление клиента
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477705"
---
# <a name="delete-tenant"></a><span data-ttu-id="b41f9-102">Удаление клиента</span><span class="sxs-lookup"><span data-stu-id="b41f9-102">Delete tenant</span></span>

<span data-ttu-id="b41f9-103">Чтобы удалить Azure AD, убедитесь, что:</span><span class="sxs-lookup"><span data-stu-id="b41f9-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="b41f9-104">Вы являетесь глобальным администратором каталога.</span><span class="sxs-lookup"><span data-stu-id="b41f9-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="b41f9-105">Вы не вошли в систему с помощью учетной записи, имеющей каталог по умолчанию, например contoso.onmicrosoft.com, в учетной записи с входом в систему, например admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b41f9-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="b41f9-106">Перед удалением удалите все активные приложения в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b41f9-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="b41f9-107">Чтобы удалить активные приложения, перейдите к разделу Регистрация приложений и удалите существующие приложения.</span><span class="sxs-lookup"><span data-stu-id="b41f9-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="b41f9-108">Нет активных подписок для всех служб Microsoft Online, таких как Microsoft Azure, Office 365 или Azure AD Premium, связанных с каталогом.</span><span class="sxs-lookup"><span data-stu-id="b41f9-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="b41f9-109">Перенесите свои подписки или упростите отмену активных подписок с помощью поддержки и выставления счетов в Azure.</span><span class="sxs-lookup"><span data-stu-id="b41f9-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="b41f9-110">Узнайте больше о том, как отказаться от использования подписок на Office 365 и Azure.</span><span class="sxs-lookup"><span data-stu-id="b41f9-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="b41f9-111">Рекомендации по связыванию или добавлению существующей подписки на клиент можно узнать в статье [связывание или Добавление подписки Azure к клиенту Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b41f9-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="b41f9-112">Отсутствует активная лицензия.</span><span class="sxs-lookup"><span data-stu-id="b41f9-112">There are no Active license.</span></span> <span data-ttu-id="b41f9-113">Чтобы удалить лицензии, ознакомьтесь со статьей [Удаление подписки для удаления лицензии](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="b41f9-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="b41f9-114">В каталоге нет других активных пользователей, кроме глобального администратора при попытке удалить Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b41f9-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="b41f9-115">Удалите все остальные активные пользователи, Кроме того, необходимо удалить все зависимости от имени пользовательского домена в клиенте, например пользователей, созданных с помощью admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b41f9-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="b41f9-116">Для получения более подробных инструкций:</span><span class="sxs-lookup"><span data-stu-id="b41f9-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="b41f9-117">Delete "Azure Active Directory" или "Subscription", ознакомьтесь со статьей [Удаление Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="b41f9-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="b41f9-118">Удалению приложений в каталоге можно узнать в статье [Удаление приложений](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="b41f9-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
