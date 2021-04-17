---
title: Active Directory, не синхронизируются
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822864"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="39ad9-102">Active Directory, не синхронизируются</span><span class="sxs-lookup"><span data-stu-id="39ad9-102">Active Directory not syncing</span></span>

<span data-ttu-id="39ad9-103">Если вы получаете ошибки синхронизации, такие как "не последняя синхронизация", или обратите внимание, что состояние синхронизации каталогов на портале администрирования Office гласит: "Последняя синхронизация была выполнена более 3 дней назад", возможно, что AADConnect имеет неправильные параметры или недостаточно разрешений для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="39ad9-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="39ad9-104">Переустановка AADConnect с помощью экспресс-параметров может быстро устранить проблему:</span><span class="sxs-lookup"><span data-stu-id="39ad9-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="39ad9-105">[Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="39ad9-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="39ad9-106">[Следуйте инструкциям по экспресс-установке.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="39ad9-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="39ad9-107">Дополнительные сведения об учетных записях службы AADConnect см. в статье [Azure AD Connect: учетные записи и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="39ad9-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
