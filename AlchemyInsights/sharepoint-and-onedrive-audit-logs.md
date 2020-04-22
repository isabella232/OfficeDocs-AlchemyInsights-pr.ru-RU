---
title: Отчеты по классическим журналам аудита SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741978"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="fb2bd-102">Журналы аудита SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="fb2bd-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="fb2bd-103">Классические журналы аудита SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb2bd-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="fb2bd-104">Прежний аудит SPO был перенесен в единый журнал аудита (UAL).</span><span class="sxs-lookup"><span data-stu-id="fb2bd-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="fb2bd-105">Все устаревшие отчеты об аудите SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="fb2bd-106">Основные изменения:</span><span class="sxs-lookup"><span data-stu-id="fb2bd-106">Key changes:</span></span>

* <span data-ttu-id="fb2bd-107">Фильтрация недоступна в качестве возможности.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="fb2bd-108">Выбор определенных событий для аудита недоступен.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="fb2bd-109">В [этом документе](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) приведен полный список событий аудита, доступных по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="fb2bd-110">Параметр **Расположение** в разделе **настроенные отчеты** недоступен.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="fb2bd-111">Параметр **Открытие или скачивание событий документов** недоступен.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="fb2bd-112">Настройка параметров аудита для семейства веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="fb2bd-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="fb2bd-113">Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="fb2bd-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="fb2bd-114">Включение и выключение ведения журнала единого аудита</span><span class="sxs-lookup"><span data-stu-id="fb2bd-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="fb2bd-115">В SharePoint или OneDrive дополнительные настройки не требуются.</span><span class="sxs-lookup"><span data-stu-id="fb2bd-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="fb2bd-116">Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:</span><span class="sxs-lookup"><span data-stu-id="fb2bd-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="fb2bd-117">Действия, связанные с файлами и страницами</span><span class="sxs-lookup"><span data-stu-id="fb2bd-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="fb2bd-118">Действия, связанные с папками</span><span class="sxs-lookup"><span data-stu-id="fb2bd-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="fb2bd-119">Действия, связанные с общим доступом и запросами на доступ</span><span class="sxs-lookup"><span data-stu-id="fb2bd-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="fb2bd-120">Действия, связанные с синхронизацией</span><span class="sxs-lookup"><span data-stu-id="fb2bd-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="fb2bd-121">Действия, связанные с администрированием сайта</span><span class="sxs-lookup"><span data-stu-id="fb2bd-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="fb2bd-122">Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="fb2bd-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
