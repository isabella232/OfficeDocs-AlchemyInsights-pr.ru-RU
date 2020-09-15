---
title: Добавление внешних пользователей в группу рассылки
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663526"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="955e7-102">Добавление внешних пользователей в группу рассылки</span><span class="sxs-lookup"><span data-stu-id="955e7-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="955e7-103">Добавление внешнего контакта в группу рассылки (рассылки) состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="955e7-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="955e7-104">Создайте почтовый контакт для внешнего пользователя:</span><span class="sxs-lookup"><span data-stu-id="955e7-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="955e7-105">В центре администрирования перейдите на **Users**  >  страницу[контактов](https://admin.microsoft.com/adminportal/home#/Contact) пользователей.</span><span class="sxs-lookup"><span data-stu-id="955e7-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="955e7-106">Нажмите кнопку **Добавить контакт**.</span><span class="sxs-lookup"><span data-stu-id="955e7-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="955e7-107">Введите сведения о контакте и нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="955e7-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="955e7-108">Добавьте почтовый контакт в вашу подсистему рассылки:</span><span class="sxs-lookup"><span data-stu-id="955e7-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="955e7-109">В центре администрирования перейдите на **Groups**  >  страницу[группы](https://admin.microsoft.com/adminportal/home#/groups) группы.</span><span class="sxs-lookup"><span data-stu-id="955e7-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="955e7-110">Найдите группу рассылки, в которую нужно добавить внешнего пользователя, и выберите ее, чтобы открыть диалоговое окно редактирования.</span><span class="sxs-lookup"><span data-stu-id="955e7-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="955e7-111">На вкладке **Участники** выберите **Просмотр всех участников и управление ими**.</span><span class="sxs-lookup"><span data-stu-id="955e7-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="955e7-112">Нажмите кнопку **Добавить участников**.</span><span class="sxs-lookup"><span data-stu-id="955e7-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="955e7-113">Выберите почтовый контакт, созданный на предыдущем шаге, а затем нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="955e7-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="955e7-114">Если после выполнения этих действий внешние пользователи не смогут отправлять сообщения в группу рассылки или не получали сообщения от него, может быть, что эта рассылка помечена так, чтобы разрешать электронную почту только от внутренних пользователей.</span><span class="sxs-lookup"><span data-stu-id="955e7-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="955e7-115">Вы можете проверить эту конфигурацию и устранить ее, следуя указаниям, приведенным [здесь](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="955e7-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="955e7-116">**Примечание:** Эти инструкции не применяются, если типом вашей группы является "Microsoft 365 группа", а не "группа рассылки".</span><span class="sxs-lookup"><span data-stu-id="955e7-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="955e7-117">В этом случае внешний пользователь можно добавить непосредственно в группу из Outlook.</span><span class="sxs-lookup"><span data-stu-id="955e7-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="955e7-118">Подробные сведения о гостевых группах Microsoft 365, а также инструкции по добавлению внешних гостей можно найти в [этой статье](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="955e7-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  