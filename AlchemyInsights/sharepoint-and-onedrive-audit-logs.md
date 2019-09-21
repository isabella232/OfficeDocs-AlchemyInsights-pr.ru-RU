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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Журналы аудита SharePoint и OneDrive

**Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям**

- [Включение и выключение ведения журнала единого аудита](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

В SharePoint или OneDrive дополнительные настройки не требуются.

- Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:

    - [Действия с файлами и страницами](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Действия с папками](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Общие действия и запросы на доступ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Действия синхронизации](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Действия по администрированию сайта](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Классические журналы аудита SharePoint**

Мы перенесли прежний аудит SPO в журнал единого аудита (UAL). Это означает, что все устаревшие отчеты аудита SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.

Основные изменения:

- Усечение в качестве возможности недоступно.
- Раздел, в котором выбираются конкретные события для аудита, недоступен. Обратитесь к [этому документу](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , чтобы получить полный список отслеживаемых событий, доступных по умолчанию.
- Параметр "расположение" в разделе " **настроенные отчеты** " недоступен. 
- События "Открытие и скачивание документов" недоступны. 

