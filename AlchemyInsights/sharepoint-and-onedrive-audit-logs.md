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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068036"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="3dd73-102">Журналы аудита SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="3dd73-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="3dd73-103">**Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям**</span><span class="sxs-lookup"><span data-stu-id="3dd73-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="3dd73-104">Включение и выключение ведения журнала единого аудита</span><span class="sxs-lookup"><span data-stu-id="3dd73-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="3dd73-105">В SharePoint или OneDrive дополнительные настройки не требуются.</span><span class="sxs-lookup"><span data-stu-id="3dd73-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="3dd73-106">Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:</span><span class="sxs-lookup"><span data-stu-id="3dd73-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="3dd73-107">Действия с файлами и страницами</span><span class="sxs-lookup"><span data-stu-id="3dd73-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="3dd73-108">Действия с папками</span><span class="sxs-lookup"><span data-stu-id="3dd73-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="3dd73-109">Общие действия и запросы на доступ</span><span class="sxs-lookup"><span data-stu-id="3dd73-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="3dd73-110">Действия синхронизации</span><span class="sxs-lookup"><span data-stu-id="3dd73-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="3dd73-111">Действия по администрированию сайта</span><span class="sxs-lookup"><span data-stu-id="3dd73-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="3dd73-112">Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="3dd73-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="3dd73-113">**Классические журналы аудита SharePoint**</span><span class="sxs-lookup"><span data-stu-id="3dd73-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="3dd73-114">Мы перенесли прежний аудит SPO в журнал единого аудита (UAL).</span><span class="sxs-lookup"><span data-stu-id="3dd73-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="3dd73-115">Это означает, что все устаревшие отчеты аудита SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.</span><span class="sxs-lookup"><span data-stu-id="3dd73-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="3dd73-116">Основные изменения:</span><span class="sxs-lookup"><span data-stu-id="3dd73-116">Key changes:</span></span>

- <span data-ttu-id="3dd73-117">Усечение в качестве возможности недоступно.</span><span class="sxs-lookup"><span data-stu-id="3dd73-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="3dd73-118">Раздел, в котором выбираются конкретные события для аудита, недоступен.</span><span class="sxs-lookup"><span data-stu-id="3dd73-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="3dd73-119">Обратитесь к [этому документу](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , чтобы получить полный список отслеживаемых событий, доступных по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3dd73-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="3dd73-120">Параметр "расположение" в разделе " **настроенные отчеты** " недоступен.</span><span class="sxs-lookup"><span data-stu-id="3dd73-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="3dd73-121">События "Открытие и скачивание документов" недоступны.</span><span class="sxs-lookup"><span data-stu-id="3dd73-121">“Opening or downloading documents” events is NOT available.</span></span> 

