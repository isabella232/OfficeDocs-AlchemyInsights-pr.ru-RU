---
title: 902 (ошибки синхронизации из-за дублирования объектов)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767148"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1207a-102">Ошибки синхронизации из-за повторяющихся объектов</span><span class="sxs-lookup"><span data-stu-id="1207a-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1207a-103">При завершении синхронизации службы каталогов в Microsoft 365 может появиться одно из следующих сообщений об ошибке:</span><span class="sxs-lookup"><span data-stu-id="1207a-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="1207a-104">Не удалось обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальном каталоге.</span><span class="sxs-lookup"><span data-stu-id="1207a-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="1207a-105">Синхронизированный объект с таким же прокси-адресом уже существует в вашем каталоге Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="1207a-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="1207a-106">Не удалось обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальных службах каталогов: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1207a-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="1207a-107">Чтобы определить и устранить проблему, скачайте и запустите [средство устранения ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1207a-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="1207a-108">Дополнительные сведения см. в разделе [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1207a-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
