---
title: 2609 — хранение и обнаружение электронных данных
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994090"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="477ff-102">Не удается удалить элементы в SharePoint Online или OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="477ff-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="477ff-103">Невозможно удалить элементы из SharePoint Online или OneDrive для бизнеса, так как политика хранения, метка хранения или удержание обнаружения электронных данных применяются к сайту SharePoint или определенному элементу.</span><span class="sxs-lookup"><span data-stu-id="477ff-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="477ff-104">Сюда также не удается удалить документ, версию документа, папку, библиотеку документов, список, приложение, сайт или семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="477ff-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="477ff-105">Ниже приведено несколько примеров сообщений об ошибках, которые могут возникать при попытке удалить сохраненный элемент.</span><span class="sxs-lookup"><span data-stu-id="477ff-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="477ff-106">"Этот сайт невозможно удалить, так как он включен в политику хранения eDiscovery или хранения"</span><span class="sxs-lookup"><span data-stu-id="477ff-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="477ff-107">"Этот сайт имеет политику соответствия, настроенную на блокировку удаления"</span><span class="sxs-lookup"><span data-stu-id="477ff-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="477ff-108">"Политика соответствия сейчас блокирует удаление этого сайта"</span><span class="sxs-lookup"><span data-stu-id="477ff-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="477ff-109">"Это семейство веб-сайтов не может быть удалено, так как оно содержит сайты, включенные в удержание eDiscovery или политику хранения"</span><span class="sxs-lookup"><span data-stu-id="477ff-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="477ff-110">"Необходимо удалить все элементы в этой папке перед удалением папки"</span><span class="sxs-lookup"><span data-stu-id="477ff-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="477ff-111">"Не удается удалить версии этого элемента, так как он находится на удержании или в политике хранения"</span><span class="sxs-lookup"><span data-stu-id="477ff-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="477ff-112">"Элемент не может быть удален во время удержания"</span><span class="sxs-lookup"><span data-stu-id="477ff-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="477ff-113">"Метка, которая применяется к этому элементу, запрещает его редактирование или удаление"</span><span class="sxs-lookup"><span data-stu-id="477ff-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="477ff-114">"Список не может быть удален во время удержания или политики хранения"</span><span class="sxs-lookup"><span data-stu-id="477ff-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="477ff-115">"Невозможно удалить список, если он заблокирован или к нему применена политика хранения"</span><span class="sxs-lookup"><span data-stu-id="477ff-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="477ff-116">Чтобы удалить элементы в одном из этих сценариев, необходимо удалить политику хранения, метку хранения или удержание обнаружения электронных данных (сайт должен быть исключен из политики хранения).</span><span class="sxs-lookup"><span data-stu-id="477ff-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="477ff-117">Необходимо отключить или исключить соответствующие удержания, которые приводят к возникновению этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="477ff-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="477ff-118">После удаления политики хранения или удержания может потребоваться до 24 часов, чтобы изменения вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="477ff-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="477ff-119">Сведения о различных функциях хранения и хранения, которые можно применить к сайтам SharePoint и учетным записям OneDrive, можно найти в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="477ff-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="477ff-120">Обзор политик хранения</span><span class="sxs-lookup"><span data-stu-id="477ff-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="477ff-121">Обзор меток хранения</span><span class="sxs-lookup"><span data-stu-id="477ff-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="477ff-122">Управление удержаниями в Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="477ff-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="477ff-123">удержания электронных данных</span><span class="sxs-lookup"><span data-stu-id="477ff-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="477ff-124">Политики закрытия и удаления устаревших сайтов</span><span class="sxs-lookup"><span data-stu-id="477ff-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
