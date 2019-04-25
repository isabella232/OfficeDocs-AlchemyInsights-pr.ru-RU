---
title: Проблемы с разРешениями при миграции
ms.author: kirks
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 3cdf5909595b5b1fac9aeb00865546c1dcff5f09
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372177"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="c18d5-102">Синхронизация профилей пользователей и фотографий</span><span class="sxs-lookup"><span data-stu-id="c18d5-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="c18d5-103">**Profile Photo Synchronization** — пользователи могут заметить, что их фотография профиля не синхронизируется с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c18d5-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="c18d5-104">Или, возможно, они попытались обновить фотографию профиля, и фотография по-прежнему отображается как старая фотография.</span><span class="sxs-lookup"><span data-stu-id="c18d5-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="c18d5-105">Чтобы убедиться, что фотографии профиля отображаются должным образом, пользователю потребуется запустить синхронизацию фотографий.</span><span class="sxs-lookup"><span data-stu-id="c18d5-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="c18d5-106">Дополнительные сведения о процессе синхронизации фотографий приведены [в статье сведения о синхронизации изображений профилей в Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="c18d5-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="c18d5-107">**Синхронизация профилей** — время, необходимое для выполнения синхронизации профилей, зависит от количества изменений (работа), которые должен выполнить задание импорта AD.</span><span class="sxs-lookup"><span data-stu-id="c18d5-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="c18d5-108">При наличии большого количества изменений задание таймера выполняет большое количество действий, а изменения в приложении профиля пользователя требуют больше времени.</span><span class="sxs-lookup"><span data-stu-id="c18d5-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="c18d5-109">Если для задания таймера требуется небольшой объем работы, изменения будут отражены в приложении профилей пользователей значительно быстрее.</span><span class="sxs-lookup"><span data-stu-id="c18d5-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="c18d5-110">Дополнительные сведения о процессе синхронизации профилей приведены [в статье сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="c18d5-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="c18d5-111">**Обновление профиля в Office delve** пользователи delve могут управлять своим профилем Office 365.</span><span class="sxs-lookup"><span data-stu-id="c18d5-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="c18d5-112">Дополнительные сведения см. [в статье Просмотр и обновление профиля в Office delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="c18d5-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

