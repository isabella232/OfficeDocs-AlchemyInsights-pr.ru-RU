---
title: Восстановление удаленного файла или папки
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 2702837bff2c0a465dde2c090a44e02747cc85ec
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051078"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="b537b-102">Восстановление удаленного файла или папки</span><span class="sxs-lookup"><span data-stu-id="b537b-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="b537b-103">SharePoint Online сохраняет резервные копии всего содержимого в течение 14 дополнительных дней после фактического удаления.</span><span class="sxs-lookup"><span data-stu-id="b537b-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="b537b-104">Если содержимое не может быть восстановлено с помощью восстановления корзины или файлов, администратор может обратиться в службу поддержки Майкрософт, чтобы запросить восстановление в течение 14 дней.</span><span class="sxs-lookup"><span data-stu-id="b537b-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="b537b-105">Восстановление из резервных копий доступно только для семейств веб-сайтов и дочерних сайтов, а не для отдельных файлов, списков и библиотек.</span><span class="sxs-lookup"><span data-stu-id="b537b-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="b537b-106">При удалении элемента или сайта из SharePoint он не удаляется сразу.</span><span class="sxs-lookup"><span data-stu-id="b537b-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="b537b-107">Удаленные элементы помещаются в корзину на некоторый период времени.</span><span class="sxs-lookup"><span data-stu-id="b537b-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="b537b-108">В течение этого времени вы можете восстановить удаленные элементы в исходное расположение.</span><span class="sxs-lookup"><span data-stu-id="b537b-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="b537b-109">Дополнительные сведения см. по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="b537b-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="b537b-110">[Восстановление элементов в корзине сайта SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="b537b-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="b537b-111">Восстановление удаленных файлов и папок в OneDrive</span><span class="sxs-lookup"><span data-stu-id="b537b-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="b537b-112">Восстановление удаленного семейства веб-сайтов (включая группу, связь и другие сайты)</span><span class="sxs-lookup"><span data-stu-id="b537b-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="b537b-113">Восстановление удаленного сайта OneDrive</span><span class="sxs-lookup"><span data-stu-id="b537b-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="b537b-114">Для действий массового перезапуска, администраторы могут рассмотреть возможность использования [SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="b537b-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="b537b-115">**Функция восстановления файлов**</span><span class="sxs-lookup"><span data-stu-id="b537b-115">**Files Restore feature**</span></span>

<span data-ttu-id="b537b-116">Если многие файлы OneDrive или SharePoint будут удалены, перезаписаны, повреждены или заражены вредоносными программами, вы можете восстановить всю библиотеку OneDrive или SharePoint в прошлый раз с помощью функции восстановления файлов.</span><span class="sxs-lookup"><span data-stu-id="b537b-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="b537b-117">Восстановление библиотеки OneDrive</span><span class="sxs-lookup"><span data-stu-id="b537b-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="b537b-118">Восстановление библиотеки документов</span><span class="sxs-lookup"><span data-stu-id="b537b-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

