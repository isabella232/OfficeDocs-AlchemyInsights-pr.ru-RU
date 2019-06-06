---
title: Устранение неполадок при доступе к сообщениям
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735750"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="a0cfc-102">Устранение неполадок при доступе к сообщениям</span><span class="sxs-lookup"><span data-stu-id="a0cfc-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="a0cfc-103">Если вы получаете сообщение об отказе в доступе при попытке просмотреть сайт SharePoint Online, ознакомьтесь со статьями ниже.</span><span class="sxs-lookup"><span data-stu-id="a0cfc-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="a0cfc-104">Добавление и лицензия пользователя</span><span class="sxs-lookup"><span data-stu-id="a0cfc-104">Add and License the user</span></span>

<span data-ttu-id="a0cfc-105">Убедитесь, что вы [назначаете пользователям лицензии в Office 365 для бизнеса](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="a0cfc-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="a0cfc-106">Назначение разрешений</span><span class="sxs-lookup"><span data-stu-id="a0cfc-106">Assign Permissions</span></span>

<span data-ttu-id="a0cfc-107">Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него [назначен соответствующий уровень разрешений](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a0cfc-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="a0cfc-108">Рассмотрите возможность использования функции запросов на доступ</span><span class="sxs-lookup"><span data-stu-id="a0cfc-108">Consider using the access request feature</span></span>

<span data-ttu-id="a0cfc-109">Функция [запросов на доступ](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения.</span><span class="sxs-lookup"><span data-stu-id="a0cfc-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="a0cfc-110">Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом</span><span class="sxs-lookup"><span data-stu-id="a0cfc-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="a0cfc-111">Существует несколько сценариев, в которых функция "разрешить пользовательский сценарий" может привести к отказу в доступе.</span><span class="sxs-lookup"><span data-stu-id="a0cfc-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="a0cfc-112">Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции.</span><span class="sxs-lookup"><span data-stu-id="a0cfc-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a0cfc-113">Посетите, разрешите [или запретите использование настраиваемого скрипта](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="a0cfc-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="a0cfc-114">Примечание. Если сайт OneDrive или SharePoint недоступен для нескольких пользователей, у которых ранее был доступ, может возникнуть временная ошибка службы.</span><span class="sxs-lookup"><span data-stu-id="a0cfc-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a0cfc-115">[Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a0cfc-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

