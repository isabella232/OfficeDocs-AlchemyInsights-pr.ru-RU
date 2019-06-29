---
title: Выбытие служб Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359373"
---
# <a name="access-services-retirement"></a><span data-ttu-id="f9162-102">Выбытие служб Access</span><span class="sxs-lookup"><span data-stu-id="f9162-102">Access services retirement</span></span>

<span data-ttu-id="f9162-103">Как мы изначально объявили в MC97576, в марте 2017 и продолжали общаться в течение прошлого года службы доступа отменяются от Office 365.</span><span class="sxs-lookup"><span data-stu-id="f9162-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="f9162-104">Следующим этапом в этом процессе будет удаление веб-баз данных Access, использующих списки SharePoint в качестве базового хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="f9162-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="f9162-105">**Как это влияет на меня?**</span><span class="sxs-lookup"><span data-stu-id="f9162-105">**How does this affect me?**</span></span>

<span data-ttu-id="f9162-106">Начиная с 2019 июня мы не будем создавать новые базы данных Access в SharePoint Online, а также завершать работу службы и остальных приложений на 2020 апреля.</span><span class="sxs-lookup"><span data-stu-id="f9162-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="f9162-107">**Что нужно сделать, чтобы подготовиться к этому изменению?**</span><span class="sxs-lookup"><span data-stu-id="f9162-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="f9162-108">Мы рекомендуем создать план перехода для веб-баз данных доступа в Организации.</span><span class="sxs-lookup"><span data-stu-id="f9162-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="f9162-109">Администраторы могут использовать [сканер приложения Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для получения перечня приложений Access, которые используются сайтами.</span><span class="sxs-lookup"><span data-stu-id="f9162-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="f9162-110">Существует несколько способов переноса данных веб-баз данных Access:</span><span class="sxs-lookup"><span data-stu-id="f9162-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="f9162-111">Импорт в локальную базу данных Access (. ACCDB) или в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="f9162-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="f9162-112">Мы также рекомендуем изучению Microsoft PowerApps в качестве альтернативной платформы для создания бизнес-решений без кода для веб-приложений и мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9162-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>