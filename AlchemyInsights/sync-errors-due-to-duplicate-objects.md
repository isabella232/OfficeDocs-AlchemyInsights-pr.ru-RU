---
title: 902 (ошибки синхронизации из-за дублирования объектов)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781274"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="8a9e3-102">Ошибки синхронизации из-за повторяющихся объектов</span><span class="sxs-lookup"><span data-stu-id="8a9e3-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="8a9e3-103">При завершении синхронизации службы каталогов может появиться одно из следующих сообщений об ошибке:</span><span class="sxs-lookup"><span data-stu-id="8a9e3-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="8a9e3-104">Не удалось обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальном каталоге.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="8a9e3-105">Синхронизированный объект с таким же прокси-адресом уже существует в вашем каталоге Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="8a9e3-106">Не удалось обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальных службах каталогов: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="8a9e3-107">Чтобы определить и устранить проблему, скачайте и запустите [средство устранения ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="8a9e3-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="8a9e3-108">Дополнительные сведения см. в разделе [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="8a9e3-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

