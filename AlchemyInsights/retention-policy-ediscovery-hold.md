---
title: 2609 — хранение и обнаружение электронных данных
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727904"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="04014-102">Не удается удалить элементы в SharePoint Online или OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="04014-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="04014-103">Невозможно удалить элементы из SharePoint Online или OneDrive для бизнеса, так как политика хранения, метка хранения или удержание обнаружения электронных данных применяются к сайту SharePoint или определенному элементу.</span><span class="sxs-lookup"><span data-stu-id="04014-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="04014-104">Сюда также не удается удалить документ, версию документа, папку, библиотеку документов, список, приложение, сайт или семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="04014-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="04014-105">Чтобы удалить элементы в одном из этих сценариев, необходимо удалить политику хранения, метку хранения или удержание обнаружения электронных данных (сайт должен быть исключен из политики хранения).</span><span class="sxs-lookup"><span data-stu-id="04014-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="04014-106">Необходимо отключить или исключить соответствующие удержания, которые приводят к возникновению этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="04014-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="04014-107">После удаления политики хранения или удержания может потребоваться до 24 часов, чтобы изменения вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="04014-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="04014-108">Сведения о различных функциях хранения и хранения, которые можно применить к сайтам SharePoint и учетным записям OneDrive, можно найти в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="04014-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="04014-109">Обзор политик хранения</span><span class="sxs-lookup"><span data-stu-id="04014-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="04014-110">Обзор меток хранения</span><span class="sxs-lookup"><span data-stu-id="04014-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="04014-111">Управление удержаниями в Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="04014-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="04014-112">удержания электронных данных</span><span class="sxs-lookup"><span data-stu-id="04014-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="04014-113">Политики закрытия и удаления устаревших сайтов</span><span class="sxs-lookup"><span data-stu-id="04014-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)