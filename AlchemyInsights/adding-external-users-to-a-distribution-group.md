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
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398471"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="a72c1-102">Добавление внешних пользователей в группу рассылки</span><span class="sxs-lookup"><span data-stu-id="a72c1-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="a72c1-103">Добавление внешнего контакта в группу рассылки (рассылки) состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="a72c1-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="a72c1-104">Создайте почтовый контакт для внешнего пользователя:</span><span class="sxs-lookup"><span data-stu-id="a72c1-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="a72c1-105">Щелкните [здесь](https://admin.microsoft.com/adminportal/home#/Contact) , чтобы перейти на страницу "Изменение контакта" на портале администрирования.</span><span class="sxs-lookup"><span data-stu-id="a72c1-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="a72c1-106">Нажмите кнопку **Добавить контакт**.</span><span class="sxs-lookup"><span data-stu-id="a72c1-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="a72c1-107">Введите сведения о контакте и нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="a72c1-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="a72c1-108">Добавьте почтовый контакт в вашу подсистему рассылки:</span><span class="sxs-lookup"><span data-stu-id="a72c1-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="a72c1-109">Щелкните [здесь](https://admin.microsoft.com/adminportal/home#/groups) , чтобы перейти на страницу "группы".</span><span class="sxs-lookup"><span data-stu-id="a72c1-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="a72c1-110">Найдите группу рассылки, в которую нужно добавить внешнего пользователя, и щелкните ее, чтобы открыть диалоговое окно редактирования.</span><span class="sxs-lookup"><span data-stu-id="a72c1-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="a72c1-111">Нажмите кнопку **Edit (изменить** ) в списке Members ( **Участники** ).</span><span class="sxs-lookup"><span data-stu-id="a72c1-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="a72c1-112">Нажмите кнопку **Добавить участников**.</span><span class="sxs-lookup"><span data-stu-id="a72c1-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="a72c1-113">Выберите почтовый контакт, созданный на предыдущем шаге, и нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="a72c1-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="a72c1-114">Даже после выполнения этих действий внешние пользователи не могут отправлять сообщения в группу рассылки или не получать их из него, возможно, эта рассылка помечена так, чтобы разрешать сообщения только от внутренних пользователей.</span><span class="sxs-lookup"><span data-stu-id="a72c1-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="a72c1-115">Вы можете проверить эту конфигурацию и устранить ее, следуя указаниям на этой [странице](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span><span class="sxs-lookup"><span data-stu-id="a72c1-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="a72c1-116">**Примечание:** Эти инструкции не применяются, если типом вашей группы является "Группа Office 365", а не "группа рассылки".</span><span class="sxs-lookup"><span data-stu-id="a72c1-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="a72c1-117">В этом случае внешний пользователь можно добавить непосредственно в группу из Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="a72c1-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="a72c1-118">Подробное описание групп гостей группы Office 365, а также инструкции по добавлению внешних гостей можно найти в [этой статье](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="a72c1-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

