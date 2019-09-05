---
title: Современный сайт в качестве корневого сайта
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753917"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="ceb46-102">Современный сайт в качестве корневого сайта</span><span class="sxs-lookup"><span data-stu-id="ceb46-102">Modern site as root site</span></span>

<span data-ttu-id="ceb46-103">Мы начали выгрузить новую функцию, которая позволит вам [заменить корневой сайт классического сайта на современный сайт](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="ceb46-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="ceb46-104">Используйте [командлет Invoke-споситесвап](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) для замены расположения сайта на другой сайт при архивации исходного сайта.</span><span class="sxs-lookup"><span data-stu-id="ceb46-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="ceb46-105">Доступно как для сайта группы (не для подключения к группе), так и для сайта для общения.</span><span class="sxs-lookup"><span data-stu-id="ceb46-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="ceb46-106">Не удаляйте классического корневого сайта для создания современного информационного сайта.</span><span class="sxs-lookup"><span data-stu-id="ceb46-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="ceb46-107">Корпорация Майкрософт не поддерживает этот параметр.</span><span class="sxs-lookup"><span data-stu-id="ceb46-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="ceb46-108">Удаление корневого сайта сделает все сайты SharePoint в Организации недоступными для всех пользователей, пока не восстановите сайт или не создаст новый сайт с тем же URL-адресом.</span><span class="sxs-lookup"><span data-stu-id="ceb46-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="ceb46-109">Мы будем связывать эту функцию с помощью центра сообщений.</span><span class="sxs-lookup"><span data-stu-id="ceb46-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="ceb46-110">Следует ожидать, что компонент будет включен в клиенте в ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="ceb46-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="ceb46-111">Известные проблемы с заменой сайтов</span><span class="sxs-lookup"><span data-stu-id="ceb46-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="ceb46-112">Целевой сайт может возвращать сообщение об ошибке "not found" (HTTP 404) в течение короткого периода времени.</span><span class="sxs-lookup"><span data-stu-id="ceb46-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="ceb46-113">Чтобы обновить индекс поиска, необходимо выполнить повторный обход контента.</span><span class="sxs-lookup"><span data-stu-id="ceb46-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="ceb46-114">Шаг вручную не требуется, это будет сделано автоматически.</span><span class="sxs-lookup"><span data-stu-id="ceb46-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="ceb46-115">Все, что зависит от "статических" ссылок (таких как файлы синхронизации файлов и файлов OneNote), необходимо исправить вручную.</span><span class="sxs-lookup"><span data-stu-id="ceb46-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="ceb46-116">Возможно, для сайтов Project Server необходимо проверить, что они все еще связаны должным образом.</span><span class="sxs-lookup"><span data-stu-id="ceb46-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
