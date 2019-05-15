---
title: Выбытие служб Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973944"
---
# <a name="access-services-retirement"></a><span data-ttu-id="c7546-102">Выбытие служб Access</span><span class="sxs-lookup"><span data-stu-id="c7546-102">Access services retirement</span></span>

<span data-ttu-id="c7546-103">Как мы изначально объявили в MC97576, в марте 2017 и продолжали общаться в течение прошлого года службы доступа отменяются от Office 365.</span><span class="sxs-lookup"><span data-stu-id="c7546-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="c7546-104">Следующим этапом в этом процессе будет удаление веб-баз данных Access, использующих списки SharePoint в качестве базового хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="c7546-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="c7546-105">Как это влияет на меня?</span><span class="sxs-lookup"><span data-stu-id="c7546-105">How does this affect me?</span></span>

<span data-ttu-id="c7546-106">Начиная с 2019 июня мы не будем создавать новые базы данных Access в SharePoint Online, а также завершать работу службы и остальных приложений на 2020 апреля.</span><span class="sxs-lookup"><span data-stu-id="c7546-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="c7546-107">Что нужно сделать, чтобы подготовиться к этому изменению?</span><span class="sxs-lookup"><span data-stu-id="c7546-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="c7546-108">Мы рекомендуем создать план перехода для веб-баз данных доступа в Организации.</span><span class="sxs-lookup"><span data-stu-id="c7546-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="c7546-109">Администраторы могут использовать [сканер приложения Access](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) для получения перечня приложений Access, которые используются сайтами.</span><span class="sxs-lookup"><span data-stu-id="c7546-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="c7546-110">Существует несколько способов переноса данных веб-баз данных Access:</span><span class="sxs-lookup"><span data-stu-id="c7546-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="c7546-111">Импорт в локальную базу данных Access (. ACCDB) или в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="c7546-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="c7546-112">Мы также рекомендуем изучению Microsoft PowerApps в качестве альтернативной платформы для создания бизнес-решений без кода для веб-приложений и мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="c7546-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>