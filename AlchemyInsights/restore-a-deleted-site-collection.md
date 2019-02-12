---
title: Восстановление удаленного семейства сайтов
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 22fb513771abc1a604a347204bac268771cb9e37
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29940009"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d33ac-102">Восстановление удаленного семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="d33ac-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d33ac-p101">Когда администратор удаляет семейства классический веб-сайтов, оно переводится в корзиной семейства сайтов, где будет храниться на 93 дней перед окончательным удалением. Для восстановления семейства веб-сайтов:</span><span class="sxs-lookup"><span data-stu-id="d33ac-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="d33ac-105">В классический Центр администрирования SharePoint щелкните **Корзина** на ленте.</span><span class="sxs-lookup"><span data-stu-id="d33ac-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d33ac-106">Установите флажок рядом с элементом коллекции веб-сайтов, которые необходимо восстановить.</span><span class="sxs-lookup"><span data-stu-id="d33ac-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d33ac-107">Нажмите кнопку **Восстановить удаленные элементы**.</span><span class="sxs-lookup"><span data-stu-id="d33ac-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d33ac-p102">Чтобы восстановить удаленные связи сайтов, можно использовать новый Предварительный просмотр центра администрирования SharePoint. В противном случае необходимо с помощью PowerShell. Чтобы восстановить сайт, который относится к группе Office 365, необходимо восстановить группы в центре администрирования Exchange. Группы могут быть восстановлены в течение 30 дней после их удалением.</span><span class="sxs-lookup"><span data-stu-id="d33ac-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

