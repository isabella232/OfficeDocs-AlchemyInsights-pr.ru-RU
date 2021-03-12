---
title: 902 (Ошибки синхронизации из-за дублирующихся объектов)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708075"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="704b2-102">Ошибки синхронизации из-за дублирующихся объектов</span><span class="sxs-lookup"><span data-stu-id="704b2-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="704b2-103">Вы можете получить одно из следующих сообщений об ошибке после завершения синхронизации каталогов в Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="704b2-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="704b2-104">Невозможно обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальном каталоге.</span><span class="sxs-lookup"><span data-stu-id="704b2-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="704b2-105">Синхронизированный объект с тем же прокси-адресом уже существует в Microsoft Online Services каталоге.</span><span class="sxs-lookup"><span data-stu-id="704b2-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="704b2-106">Невозможно обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальных службах каталогов: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="704b2-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="704b2-107">Чтобы определить и устранить проблему, скачайте и запустите средство исправления ошибок [IdFix DirSync.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="704b2-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="704b2-108">Дополнительные сведения см. в [kB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="704b2-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
