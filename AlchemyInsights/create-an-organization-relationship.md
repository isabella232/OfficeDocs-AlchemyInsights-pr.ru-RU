---
title: Создание связи организации, чтобы разрешить пользователям взаимодействовать с другой организацией
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854044"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="ea1bf-102">Создание связи организации, чтобы разрешить пользователям взаимодействовать с другой организацией</span><span class="sxs-lookup"><span data-stu-id="ea1bf-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="ea1bf-103">На панели мониторинга Центра администрирования Microsoft 365 выберите **Администрирование** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="ea1bf-104">Перейдите в раздел **Организация** > **Общий доступ**.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="ea1bf-105">В разделе **Общий доступ к организации** нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="ea1bf-106">В окне **Новая связь организации** в поле **Имя связи** введите понятное имя связи.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="ea1bf-107">В поле **Домены, которым предоставлен общий доступ** введите домен для внешней организации Office 365 или локальной организации Exchange, которым нужно предоставить возможность просмотра ваших календарей.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="ea1bf-108">Если требуется ввести более одного домена, разделяйте их имена запятыми.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="ea1bf-109">Например, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="ea1bf-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="ea1bf-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="ea1bf-112">Для настройки уровня доступа к сведениям о занятости выберите одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="ea1bf-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="ea1bf-113">**Календарных данных о занятости только по времени**</span><span class="sxs-lookup"><span data-stu-id="ea1bf-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="ea1bf-114">**Календарные данные о занятости со временем, темой и местом**</span><span class="sxs-lookup"><span data-stu-id="ea1bf-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="ea1bf-115">Чтобы указать, какие пользователи могут предоставлять общий доступ к сведениям о доступности в календаре, выберите один из указанных ниже вариантов.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="ea1bf-116">**Все в организации**</span><span class="sxs-lookup"><span data-stu-id="ea1bf-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="ea1bf-117">**Заданная группа безопасности**</span><span class="sxs-lookup"><span data-stu-id="ea1bf-117">**A specified security group**</span></span>  

<span data-ttu-id="ea1bf-118">Щелкните **Обзор**, чтобы выбрать из списка группу безопасности, затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="ea1bf-119">Нажмите кнопку **Сохранить**, чтобы создать связь организации.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="ea1bf-120">**Примечание**. Межклиентские конфигурации не поддерживают просмотр сведений о доступности личных контактов.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="ea1bf-121">Чтобы просматривать сведения о доступности, контакты должны быть включены в глобальный список адресов.</span><span class="sxs-lookup"><span data-stu-id="ea1bf-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="ea1bf-122">**Полные сведения по этой теме см. в статье:**</span><span class="sxs-lookup"><span data-stu-id="ea1bf-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="ea1bf-123">Создание связи организации в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ea1bf-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="ea1bf-124">Изменение связи организации в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ea1bf-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="ea1bf-125">Удаление связи организации в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ea1bf-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
