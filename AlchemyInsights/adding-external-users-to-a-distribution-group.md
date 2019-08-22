---
title: Добавление внешних пользователей в группу рассылки
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494540"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="13854-102">Добавить внешних пользователей в группу рассылки?</span><span class="sxs-lookup"><span data-stu-id="13854-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="13854-103">Добавление внешнего контакта в группу рассылки (рассылки) состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="13854-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="13854-104">Создайте почтовый контакт для внешнего пользователя:</span><span class="sxs-lookup"><span data-stu-id="13854-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="13854-105">В центре администрирования перейдите на страницу[контактов](https://admin.microsoft.com/adminportal/home#/Contact) **пользователей** > .</span><span class="sxs-lookup"><span data-stu-id="13854-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="13854-106">Нажмите кнопку **Добавить контакт**.</span><span class="sxs-lookup"><span data-stu-id="13854-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="13854-107">Введите сведения о контакте и нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="13854-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="13854-108">Добавьте почтовый контакт в вашу подсистему рассылки:</span><span class="sxs-lookup"><span data-stu-id="13854-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="13854-109">В центре администрирования перейдите на страницу[группы](https://admin.microsoft.com/adminportal/home#/groups) **группы** > .</span><span class="sxs-lookup"><span data-stu-id="13854-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="13854-110">Найдите группу рассылки, в которую нужно добавить внешнего пользователя, и выберите ее, чтобы открыть диалоговое окно редактирования.</span><span class="sxs-lookup"><span data-stu-id="13854-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="13854-111">На вкладке **Участники** выберите **Просмотр всех участников и управление ими**.</span><span class="sxs-lookup"><span data-stu-id="13854-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="13854-112">Нажмите кнопку **Добавить участников**.</span><span class="sxs-lookup"><span data-stu-id="13854-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="13854-113">Выберите почтовый контакт, созданный на предыдущем шаге, а затем нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="13854-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="13854-114">Если после выполнения этих действий внешние пользователи не смогут отправлять сообщения в группу рассылки или не получали сообщения от него, может быть, что эта рассылка помечена так, чтобы разрешать электронную почту только от внутренних пользователей.</span><span class="sxs-lookup"><span data-stu-id="13854-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="13854-115">Вы можете проверить эту конфигурацию и устранить ее, следуя указаниям, приведенным [здесь](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="13854-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="13854-116">**Примечание:** Эти инструкции не применяются, если типом вашей группы является "Группа Office 365", а не "группа рассылки".</span><span class="sxs-lookup"><span data-stu-id="13854-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="13854-117">В этом случае внешний пользователь можно добавить непосредственно в группу из Outlook.</span><span class="sxs-lookup"><span data-stu-id="13854-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="13854-118">Подробные сведения о группах Office 365 для гостей, а также инструкции по добавлению внешних гостей можно найти в [этой статье](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="13854-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  