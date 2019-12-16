---
title: Сообщение "только для чтения" для обслуживания при попытке использовать SharePoint или OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051294"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="d1864-102">Сообщение "только для чтения" для обслуживания при попытке использовать SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1864-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="d1864-103">При попытке использовать SharePoint или OneDrive для выполнения одного из следующих сценариев пользователи могут получить сообщение об **обслуживании, доступное только для чтения** .</span><span class="sxs-lookup"><span data-stu-id="d1864-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="d1864-104">Запланированные или активные действия по обслуживанию.</span><span class="sxs-lookup"><span data-stu-id="d1864-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="d1864-105">Проверьте их, перейдя в [Центр сообщений](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="d1864-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="d1864-106">Высокоприоритетный инцидент Active Service, который может возникать.</span><span class="sxs-lookup"><span data-stu-id="d1864-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="d1864-107">Проверьте наличие помощников и инцидентов, перейдя к [работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d1864-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="d1864-108">Дополнительный сценарий восстановления с автовосстановлением, который может происходить из-за непредвиденных событий на серверах, которые могут быть последними менее чем на 30 минут.</span><span class="sxs-lookup"><span data-stu-id="d1864-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="d1864-109">Не существует центра сообщений или сообщений о работоспособности службы для этих незначительных восстановлений, но вам следует вернуться к нормальному началу работы.</span><span class="sxs-lookup"><span data-stu-id="d1864-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="d1864-110">В очень редких случаях мы наблюдали, что существует один из трех указанных выше сценариев, а служба восстановлена, но кэш браузера пользователей не был очищен.</span><span class="sxs-lookup"><span data-stu-id="d1864-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="d1864-111">Перед переходом на сайт попробуйте очистить кэш браузера.</span><span class="sxs-lookup"><span data-stu-id="d1864-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="d1864-112">В браузере Microsoft Edge выберите **Параметры**, а затем выберите **Конфиденциальность и безопасность**.</span><span class="sxs-lookup"><span data-stu-id="d1864-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="d1864-113">В разделе **очистить обзор**выберите **команду выбрать, что нужно очистить**.</span><span class="sxs-lookup"><span data-stu-id="d1864-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="d1864-114">Выберите **файлы cookie и сохраненные данные веб-сайта**, а затем нажмите кнопку **очистить**.</span><span class="sxs-lookup"><span data-stu-id="d1864-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="d1864-115">Эти действия могут отличаться при использовании других браузеров, таких как Mozilla Firefox или Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="d1864-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="d1864-116">Кроме того, можно открыть сайт SharePoint или OneDrive в новом окне InPrivate.</span><span class="sxs-lookup"><span data-stu-id="d1864-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>