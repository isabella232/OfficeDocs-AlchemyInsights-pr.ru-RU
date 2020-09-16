---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771257"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="80604-102">SharePoint или OneDrive работает медленнее, недоступно или недоступно для нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="80604-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="80604-103">Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы.</span><span class="sxs-lookup"><span data-stu-id="80604-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="80604-104">[Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="80604-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="80604-105">**Добавление и лицензия пользователя**</span><span class="sxs-lookup"><span data-stu-id="80604-105">**Add and license the user**</span></span>

<span data-ttu-id="80604-106">Убедитесь, что вы [назначаете пользователям лицензии в Microsoft 365 для бизнеса](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="80604-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="80604-107">**Назначение разрешений**</span><span class="sxs-lookup"><span data-stu-id="80604-107">**Assign Permissions**</span></span>

<span data-ttu-id="80604-108">Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него назначен [соответствующий уровень разрешений](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="80604-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="80604-109">**Рассмотрите возможность использования функции запросов на доступ**</span><span class="sxs-lookup"><span data-stu-id="80604-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="80604-110">[Функция запросов на доступ](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения.</span><span class="sxs-lookup"><span data-stu-id="80604-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="80604-111">**Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом**</span><span class="sxs-lookup"><span data-stu-id="80604-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="80604-112">Существуют некоторые сценарии, в которых функции " *Разрешить пользовательскому сценарию* " может быть предоставлен отказ в доступе.</span><span class="sxs-lookup"><span data-stu-id="80604-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="80604-113">Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции.</span><span class="sxs-lookup"><span data-stu-id="80604-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="80604-114">Воспользуйтесь [разделом разрешить или запретить пользовательский сценарий](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="80604-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

