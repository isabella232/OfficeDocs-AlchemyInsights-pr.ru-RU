---
title: Active Directory не синхронизируется
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265269"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="bbed8-102">Active Directory не синхронизируется</span><span class="sxs-lookup"><span data-stu-id="bbed8-102">Active Directory not syncing</span></span>

<span data-ttu-id="bbed8-103">При получении сообщений об ошибках синхронизации, например "нет последней синхронизации", или Обратите внимание на состояние синхронизации службы каталогов на портале администрирования Office — сообщение "время последней синхронизации больше 3 дней назад", может быть неправильные параметры AADConnect или недостаточно разрешения для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bbed8-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="bbed8-104">Переустановка AADConnect с помощью Express Settings может ускорить решение проблемы:</span><span class="sxs-lookup"><span data-stu-id="bbed8-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="bbed8-105">[Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="bbed8-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="bbed8-106">[Следуйте инструкциям по установке Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="bbed8-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="bbed8-107">Дополнительные сведения об учетных записях служб AADConnect можно найти в статье [Azure AD Connect: accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="bbed8-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
