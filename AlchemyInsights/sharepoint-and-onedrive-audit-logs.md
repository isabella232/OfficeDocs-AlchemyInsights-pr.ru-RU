---
title: Отчеты по классическим журналам аудита SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992631"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="3027f-102">Журналы аудита SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="3027f-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="3027f-103">Классические журналы аудита SharePoint</span><span class="sxs-lookup"><span data-stu-id="3027f-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="3027f-104">Прежний аудит SPO был перенесен в единый журнал аудита (UAL).</span><span class="sxs-lookup"><span data-stu-id="3027f-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="3027f-105">Все устаревшие отчеты об аудите SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.</span><span class="sxs-lookup"><span data-stu-id="3027f-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="3027f-106">Основные изменения:</span><span class="sxs-lookup"><span data-stu-id="3027f-106">Key changes:</span></span>

* <span data-ttu-id="3027f-107">Фильтрация недоступна в качестве возможности.</span><span class="sxs-lookup"><span data-stu-id="3027f-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="3027f-108">Выбор определенных событий для аудита недоступен.</span><span class="sxs-lookup"><span data-stu-id="3027f-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="3027f-109">В [этом документе](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) приведен полный список событий аудита, доступных по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3027f-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="3027f-110">Параметр **Расположение** в разделе **настроенные отчеты** недоступен.</span><span class="sxs-lookup"><span data-stu-id="3027f-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="3027f-111">Параметр **Открытие или скачивание событий документов** недоступен.</span><span class="sxs-lookup"><span data-stu-id="3027f-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="3027f-112">Настройка параметров аудита для семейства веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="3027f-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="3027f-113">Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="3027f-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="3027f-114">Включение и выключение ведения журнала единого аудита</span><span class="sxs-lookup"><span data-stu-id="3027f-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="3027f-115">В SharePoint или OneDrive дополнительные настройки не требуются.</span><span class="sxs-lookup"><span data-stu-id="3027f-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="3027f-116">Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:</span><span class="sxs-lookup"><span data-stu-id="3027f-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="3027f-117">Действия с файлами и страницами</span><span class="sxs-lookup"><span data-stu-id="3027f-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="3027f-118">Действия с папками</span><span class="sxs-lookup"><span data-stu-id="3027f-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="3027f-119">Общие действия и запросы на доступ</span><span class="sxs-lookup"><span data-stu-id="3027f-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="3027f-120">Действия синхронизации</span><span class="sxs-lookup"><span data-stu-id="3027f-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="3027f-121">Действия по администрированию сайта</span><span class="sxs-lookup"><span data-stu-id="3027f-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="3027f-122">Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="3027f-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
