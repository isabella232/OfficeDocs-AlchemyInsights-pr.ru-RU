---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511161"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="2d34e-102">SharePoint или OneDrive работает медленнее, недоступно или недоступно для нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="2d34e-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="2d34e-103">Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы.</span><span class="sxs-lookup"><span data-stu-id="2d34e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="2d34e-104">[Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2d34e-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="2d34e-105">**Добавление и лицензия пользователя**</span><span class="sxs-lookup"><span data-stu-id="2d34e-105">**Add and license the user**</span></span>

<span data-ttu-id="2d34e-106">Убедитесь, что вы [назначаете пользователям лицензии в Microsoft 365 для бизнеса](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="2d34e-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="2d34e-107">**Назначение разрешений**</span><span class="sxs-lookup"><span data-stu-id="2d34e-107">**Assign Permissions**</span></span>

<span data-ttu-id="2d34e-108">Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него назначен [соответствующий уровень разрешений](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="2d34e-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="2d34e-109">**Рассмотрите возможность использования функции запросов на доступ**</span><span class="sxs-lookup"><span data-stu-id="2d34e-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="2d34e-110">[Функция запросов на доступ](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения.</span><span class="sxs-lookup"><span data-stu-id="2d34e-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="2d34e-111">**Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом**</span><span class="sxs-lookup"><span data-stu-id="2d34e-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="2d34e-112">Существуют некоторые сценарии, в которых функции " *Разрешить пользовательскому сценарию* " может быть предоставлен отказ в доступе.</span><span class="sxs-lookup"><span data-stu-id="2d34e-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="2d34e-113">Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции.</span><span class="sxs-lookup"><span data-stu-id="2d34e-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="2d34e-114">Воспользуйтесь [разделом разрешить или запретить пользовательский сценарий](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="2d34e-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

