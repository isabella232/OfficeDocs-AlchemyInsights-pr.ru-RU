---
title: Управление внешними параметрами
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282833"
---
# <a name="managing-external-settings"></a><span data-ttu-id="df360-102">Управление внешними параметрами</span><span class="sxs-lookup"><span data-stu-id="df360-102">Managing External Settings</span></span>

<span data-ttu-id="df360-103">**Объявление**</span><span class="sxs-lookup"><span data-stu-id="df360-103">**Announcement**</span></span>

- <span data-ttu-id="df360-104">[Прекращение поддержки входа в WebView из Google с 4 января 2021 г.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="df360-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="df360-105">Проверьте, повлияет ли это на ваши приложения, следуя рекомендациям Google по тестированию совместимости.</span><span class="sxs-lookup"><span data-stu-id="df360-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="df360-106">Убедитесь, что при входе пользователей с помощью обычных учетных записей Google используется системное веб-представление или системный браузер.</span><span class="sxs-lookup"><span data-stu-id="df360-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="df360-107">**Управление параметрами приглашений**</span><span class="sxs-lookup"><span data-stu-id="df360-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="df360-108">Подтвердите, что вы [настроили параметры внешней совместной работы](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support), чтобы разрешить соответствующим людям отправлять приглашения.</span><span class="sxs-lookup"><span data-stu-id="df360-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="df360-109">**Управление разрешениями гостевого доступа**</span><span class="sxs-lookup"><span data-stu-id="df360-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="df360-110">Глобальные администраторы могут управлять разрешениями гостевого доступа в каталоге на портале Microsoft Azure, настроив разрешения гостевого доступа на странице параметров внешней совместной работы.</span><span class="sxs-lookup"><span data-stu-id="df360-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="df360-111">[Подробные сведения об этом параметре](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="df360-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="df360-112">Если вы хотите, чтобы гости могли получать доступ к приложениям, таким как Teams или SharePoint, убедитесь, что вы настроили эти приложения для разрешения гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="df360-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="df360-113">Подробнее о [Параметрах Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) и [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="df360-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="df360-114">**Настройка приглашений.**</span><span class="sxs-lookup"><span data-stu-id="df360-114">**Configuring invitations:**</span></span>

- <span data-ttu-id="df360-115">[Включение внешней совместной работы B2B и управление ролями приглашающих](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="df360-115">[Enable B2B external collaboration and manage who can invite guests](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- [<span data-ttu-id="df360-116">Разрешение или блокирование приглашений пользователям от определенных организаций.</span><span class="sxs-lookup"><span data-stu-id="df360-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="df360-117">**Настройка разрешенных поставщиков удостоверений:**</span><span class="sxs-lookup"><span data-stu-id="df360-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="df360-118">Федерация Google</span><span class="sxs-lookup"><span data-stu-id="df360-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="df360-119">Прямая федерация</span><span class="sxs-lookup"><span data-stu-id="df360-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="df360-120">Проверка подлинности электронной почты с помощью одноразового секретного кода</span><span class="sxs-lookup"><span data-stu-id="df360-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
