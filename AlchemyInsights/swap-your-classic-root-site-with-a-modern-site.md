---
title: Замена на классическом корневом сайте современного сайта
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749273"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="731a5-102">Замена на классическом корневом сайте современного сайта</span><span class="sxs-lookup"><span data-stu-id="731a5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="731a5-103">Если ваша среда настроена до апреля 2019, вы можете изменить свой корневой сайт на современный сайт с помощью Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="731a5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="731a5-104">Если вы хотите использовать другой сайт, который вы хотите использовать в качестве корневого сайта, вы можете заменить его на [корневой сайт](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="731a5-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="731a5-105">Используйте [командлет Invoke-споситесвап](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) для замены расположения сайта на другой сайт при архивации исходного сайта.</span><span class="sxs-lookup"><span data-stu-id="731a5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="731a5-106">Доступно как для сайта группы (не для подключения к группе), так и для сайта для общения.</span><span class="sxs-lookup"><span data-stu-id="731a5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="731a5-107">В скором времени будут представлены дополнительные возможности, которые позволят вам продолжить использовать контент на сайте, но преобразовать существующий сайт в сайт для общения.</span><span class="sxs-lookup"><span data-stu-id="731a5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="731a5-108">Эти возможности будут сведены к постепенному развертыванию.</span><span class="sxs-lookup"><span data-stu-id="731a5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="731a5-109">Продолжайте проверять центр сообщений Office 365 на наличие обновлений.</span><span class="sxs-lookup"><span data-stu-id="731a5-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="731a5-110">Известные проблемы с заменой сайтов</span><span class="sxs-lookup"><span data-stu-id="731a5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="731a5-111">Целевой сайт может возвращать сообщение об ошибке "not found" (HTTP 404) в течение короткого периода времени.</span><span class="sxs-lookup"><span data-stu-id="731a5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="731a5-112">Чтобы обновить индекс поиска, необходимо выполнить повторный обход контента.</span><span class="sxs-lookup"><span data-stu-id="731a5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="731a5-113">Выполнение действий, выполняемых вручную, не требуется — это будет сделано автоматически.</span><span class="sxs-lookup"><span data-stu-id="731a5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="731a5-114">Все, что зависит от "статических" ссылок (таких как файлы синхронизации файлов и файлов OneNote), необходимо исправить вручную.</span><span class="sxs-lookup"><span data-stu-id="731a5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="731a5-115">Если исходный сайт являлся сайтом новостей Организации, обновите URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="731a5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="731a5-116">Получение списка всех сайтов новостей Организации.</span><span class="sxs-lookup"><span data-stu-id="731a5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="731a5-117">Возможно, для сайтов Project Server необходимо проверить, что они все еще связаны должным образом.</span><span class="sxs-lookup"><span data-stu-id="731a5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





