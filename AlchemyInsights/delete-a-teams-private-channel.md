---
title: Удаление закрытого канала Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730928"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="bb74d-102">Удаление закрытого канала Teams</span><span class="sxs-lookup"><span data-stu-id="bb74d-102">Delete a Teams private channel</span></span>

<span data-ttu-id="bb74d-103">Корпорации Майкрософт известно о проблемах с удалением закрытого канала группы, если для сайта SharePoint включены политики хранения SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb74d-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="bb74d-104">Разработчики Майкрософт работают над созданием решения.</span><span class="sxs-lookup"><span data-stu-id="bb74d-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="bb74d-105">Тем временем можно воспользоваться следующими временными решениями для удаления закрытого канала.</span><span class="sxs-lookup"><span data-stu-id="bb74d-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="bb74d-106">**Исключите команду/семейство веб-сайтов из политики хранения Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="bb74d-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="bb74d-107">Перейдите на портал администрирования Office 365 и выберите **Показать все** в области навигации слева.</span><span class="sxs-lookup"><span data-stu-id="bb74d-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="bb74d-108">В разделе **Центры администрирования** перейдите на страницу **Безопасность и соответствие требованиям** > **Защита от потери данных** > **Политика**.</span><span class="sxs-lookup"><span data-stu-id="bb74d-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="bb74d-109">Определите все политики, применяемые к сайтам Sharepoint, и измените политику таким образом, чтобы сайт команды Sharepoint, содержащий закрытый канал, НЕ был включен в политику хранения.</span><span class="sxs-lookup"><span data-stu-id="bb74d-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="bb74d-110">Сохраните политику.</span><span class="sxs-lookup"><span data-stu-id="bb74d-110">Save the policy.</span></span>
    <span data-ttu-id="bb74d-111">Применение измененных параметров политики может занять до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="bb74d-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="bb74d-112">После исключения сайта можно удалить закрытый канал.</span><span class="sxs-lookup"><span data-stu-id="bb74d-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="bb74d-113">***Возможно***, вам удастся удалить закрытый канал, используя Microsoft Teams на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="bb74d-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="bb74d-114">Сведения по теме о SharePoint см. в статье [Не удается удалить элементы в SharePoint Online и в OneDrive для бизнеса](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="bb74d-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>