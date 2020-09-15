---
title: Синхронизация профилей
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801782"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="8e737-102">Когда изменения профиля синхронизируются с приложением профиля пользователя SharePoint?</span><span class="sxs-lookup"><span data-stu-id="8e737-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="8e737-103">SharePoint Online использует задание таймера импорта Active Directory (импорт AD) для импорта пользователей и групп в приложение профилей пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e737-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="8e737-104">Служба импорта Active Directory синхронизирует изменения из хранилища каталогов SharePoint Online с приложением профилей пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e737-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="8e737-105">Эти изменения обрабатываются в пакетах.</span><span class="sxs-lookup"><span data-stu-id="8e737-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="8e737-106">Задание таймера выполняется до тех пор, пока изменения не будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="8e737-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8e737-107">Время, необходимое для выполнения задания, зависит от количества изменений, которые необходимо обработать.</span><span class="sxs-lookup"><span data-stu-id="8e737-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="8e737-108">Большое количество изменений занимает больше времени.</span><span class="sxs-lookup"><span data-stu-id="8e737-108">A large number of changes takes longer.</span></span> <span data-ttu-id="8e737-109">Соглашение об уровне обслуживания (SLA) указывает на то, что изменение пользователя в каталоге SharePoint Online будет отражено в приложении профиля пользователя в течение 24 часов.</span><span class="sxs-lookup"><span data-stu-id="8e737-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="8e737-110">Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8e737-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

