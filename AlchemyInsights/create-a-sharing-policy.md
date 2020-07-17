---
title: Создание политики общего доступа, разрешающей предоставления доступа к календарям в вашей организации для внешних пользователей
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
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854045"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="5b28d-102">Создание политики общего доступа, разрешающей предоставления доступа к календарям в вашей организации для внешних пользователей</span><span class="sxs-lookup"><span data-stu-id="5b28d-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="5b28d-103">На панели мониторинга Центра администрирования Microsoft 365 выберите **Администрирование** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5b28d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="5b28d-104">Перейдите в раздел **Организация** > **Общий доступ**.</span><span class="sxs-lookup"><span data-stu-id="5b28d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="5b28d-105">В представлении списка, в разделе **Индивидуальный общий доступ** нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="5b28d-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="5b28d-106">В разделе **Создание политики общего доступа** в поле **Имя политики** введите понятное имя политики общего доступа.</span><span class="sxs-lookup"><span data-stu-id="5b28d-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="5b28d-107">Нажмите кнопку **Добавить**, чтобы определить правила общего доступа для политики.</span><span class="sxs-lookup"><span data-stu-id="5b28d-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="5b28d-108">В поле **Правило общего доступа** выберите один из следующих параметров, чтобы указать домены, которым нужно предоставить доступ:</span><span class="sxs-lookup"><span data-stu-id="5b28d-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="5b28d-109">**Общий доступ для всех доменов**</span><span class="sxs-lookup"><span data-stu-id="5b28d-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="5b28d-110">**Общий доступ для определенного домена**</span><span class="sxs-lookup"><span data-stu-id="5b28d-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="5b28d-p101">При выборе **Общий доступ для конкретного домена** введите имя домена, которому необходимо предоставить общий доступ. Чтобы ввести несколько доменов для одной политики общего доступа, сохраните настройки первого домена, а затем измените правила общего доступа для добавления других доменов.</span><span class="sxs-lookup"><span data-stu-id="5b28d-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="5b28d-113">Чтобы указать информацию, к которой нужно предоставить доступ, установите флажок **Предоставить общий доступ к папке календаря**, а затем выберите один из следующих параметров:</span><span class="sxs-lookup"><span data-stu-id="5b28d-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="5b28d-114">**Календарных данных о занятости только по времени**</span><span class="sxs-lookup"><span data-stu-id="5b28d-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="5b28d-115">**Со временем данные календаря о занятости, теме, местоположении и**</span><span class="sxs-lookup"><span data-stu-id="5b28d-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="5b28d-116">**Все данные о встрече, включая время, тему, местоположение и название**</span><span class="sxs-lookup"><span data-stu-id="5b28d-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="5b28d-117">Нажмите кнопку **Сохранить**, чтобы настроить правила для политики общего доступа.</span><span class="sxs-lookup"><span data-stu-id="5b28d-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="5b28d-118">Чтобы сделать эту политику общего доступа политикой по умолчанию для пользователей в вашей организации, установите флажок **Сделать политику политикой общего доступа по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="5b28d-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="5b28d-119">Нажмите кнопку **Сохранить**, чтобы создать политику общего доступа.</span><span class="sxs-lookup"><span data-stu-id="5b28d-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="5b28d-120">**Полные сведения по этой теме см. в статье:**</span><span class="sxs-lookup"><span data-stu-id="5b28d-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="5b28d-121">Создание политики общего доступа в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5b28d-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="5b28d-122">Применение политики общего доступа к почтовым ящикам в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5b28d-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="5b28d-123">Изменение, отключение или удаление политики общего доступа в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5b28d-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)