---
title: Синхронизация профилей
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768126"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a7813-102">Когда изменения профиля синхронизируются с приложением профиля пользователя SharePoint?</span><span class="sxs-lookup"><span data-stu-id="a7813-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a7813-103">SharePoint Online использует задание таймера импорта Active Directory (импорт AD) для импорта пользователей и групп в приложение профилей пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7813-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a7813-104">Служба импорта Active Directory синхронизирует изменения из хранилища каталогов SharePoint Online с приложением профилей пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7813-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a7813-105">Эти изменения обрабатываются в пакетах.</span><span class="sxs-lookup"><span data-stu-id="a7813-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a7813-106">Задание таймера выполняется до тех пор, пока изменения не будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="a7813-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a7813-107">Время, необходимое для выполнения задания, зависит от количества изменений, которые необходимо обработать.</span><span class="sxs-lookup"><span data-stu-id="a7813-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a7813-108">Большое количество изменений занимает больше времени.</span><span class="sxs-lookup"><span data-stu-id="a7813-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a7813-109">Соглашение об уровне обслуживания (SLA) указывает на то, что изменение пользователя в каталоге SharePoint Online будет отражено в приложении профиля пользователя в течение 24 часов.</span><span class="sxs-lookup"><span data-stu-id="a7813-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a7813-110">Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a7813-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

