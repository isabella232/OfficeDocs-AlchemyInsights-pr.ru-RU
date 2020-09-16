---
title: Устранение ошибки 404, файл не найден
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750104"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="433c7-102">Устранение ошибки 404, файл не найден</span><span class="sxs-lookup"><span data-stu-id="433c7-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="433c7-103">Сообщение об ошибке 404 получено, когда пользователи пытаются получить доступ к сайту или файлу в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="433c7-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="433c7-104">Часто это вызвано тем, что сайт или файл или группа переименованы, перемещены или удалены.</span><span class="sxs-lookup"><span data-stu-id="433c7-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="433c7-105">Например: пользователи увидят ошибку 404 при попытке доступа к корневому семейству веб-сайтов и были удалены.</span><span class="sxs-lookup"><span data-stu-id="433c7-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="433c7-106">Устранение ошибки 404 для сайта, который был переименован, перемещен или удален:</span><span class="sxs-lookup"><span data-stu-id="433c7-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="433c7-107">Для классических сайтов, существующих в классическом центре администрирования, можно ознакомиться в статье [Восстановление удаленного семейства веб-сайтов](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="433c7-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="433c7-108">Для современных сайтов (общения, подключенных к группам или других сайтов), существующих в новом центре администрирования SharePoint, ознакомьтесь со статьей [Просмотр и восстановление удаленных сайтов в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="433c7-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="433c7-109">Устранение ошибки 404 для файла (или другого элемента), который был переименован, перемещен или удален:</span><span class="sxs-lookup"><span data-stu-id="433c7-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="433c7-110">Перейдите на сайт SharePoint или OneDrive и просмотрите корзину в содержимом сайта.</span><span class="sxs-lookup"><span data-stu-id="433c7-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="433c7-111">Просмотр, [Восстановление элементов в корзине сайта SharePoint](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="433c7-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="433c7-112">Если по-прежнему не удается найти элемент, который можно искать в журнале аудита, если включено ведение журнала, [выполните поиск в журнале аудита в центре безопасности & соответствия требованиям Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="433c7-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
