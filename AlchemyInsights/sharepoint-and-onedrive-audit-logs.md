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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Журналы аудита SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Классические журналы аудита SharePoint

Прежний аудит SPO был перенесен в единый журнал аудита (UAL). Все устаревшие отчеты об аудите SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.

Основные изменения:

* Фильтрация недоступна в качестве возможности.
* Выбор определенных событий для аудита недоступен. В [этом документе](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) приведен полный список событий аудита, доступных по умолчанию.
* Параметр **Расположение** в разделе **настроенные отчеты** недоступен.
* Параметр **Открытие или скачивание событий документов** недоступен.

[Настройка параметров аудита для семейства веб-сайтов](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям

* [Включение и выключение ведения журнала единого аудита](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

В SharePoint или OneDrive дополнительные настройки не требуются.

Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:

* [Действия с файлами и страницами](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Действия с папками](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Общие действия и запросы на доступ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Действия синхронизации](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Действия по администрированию сайта](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
