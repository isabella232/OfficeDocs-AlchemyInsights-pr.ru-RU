---
title: Teams разрешают или отключают IP-видео
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670197"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="14793-102">Teams разрешают или отключают IP-видео</span><span class="sxs-lookup"><span data-stu-id="14793-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="14793-103">**Изменить или создать политику встреч**</span><span class="sxs-lookup"><span data-stu-id="14793-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="14793-104">Чтобы изменить или создать политику собрания, перейдите в **Центр администрирования Microsoft Teams > Собрания > Политики собраний**.</span><span class="sxs-lookup"><span data-stu-id="14793-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="14793-105">Выберите политику в списке или нажмите кнопку **добавить**.</span><span class="sxs-lookup"><span data-stu-id="14793-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="14793-106">Если вы создаете новую политику, укажите ее имя и описание.</span><span class="sxs-lookup"><span data-stu-id="14793-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="14793-107">Имя не может содержать специальные символы. Длина имени не должна превышать 64 символа.</span><span class="sxs-lookup"><span data-stu-id="14793-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="14793-108">Выберите параметры, затем нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="14793-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="14793-109">Например, предположим, что нужно ограничить пропускную способность собрания, в котором будет участвовать много пользователей.</span><span class="sxs-lookup"><span data-stu-id="14793-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="14793-110">Для этого следует создать новую настраиваемую политику с именем "Ограниченная пропускная способность" и отключить следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="14793-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="14793-111">В разделе **Аудио и видео**:</span><span class="sxs-lookup"><span data-stu-id="14793-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="14793-112">Отключите параметр "Разрешить запись в облаке".</span><span class="sxs-lookup"><span data-stu-id="14793-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="14793-113">Отключите параметр "Разрешить видео по IP".</span><span class="sxs-lookup"><span data-stu-id="14793-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="14793-114">Затем назначьте политику пользователям.</span><span class="sxs-lookup"><span data-stu-id="14793-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="14793-115">**Назначение пользователям политики собрания**</span><span class="sxs-lookup"><span data-stu-id="14793-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="14793-116">В Центре администрирования Microsoft Teams в области навигации слева перейдите в раздел **Пользователи**, затем щелкните пользователя.</span><span class="sxs-lookup"><span data-stu-id="14793-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="14793-117">Выберите пользователя, щелкнув слева от его имени, затем нажмите кнопку **Изменить параметры**.</span><span class="sxs-lookup"><span data-stu-id="14793-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="14793-118">В разделе **Политика собраний** выберите политику, которую нужно назначить, и нажмите кнопку **Применить**.</span><span class="sxs-lookup"><span data-stu-id="14793-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="14793-119">Дополнительные сведения см. в разделе [Управление политиками собраний в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="14793-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
