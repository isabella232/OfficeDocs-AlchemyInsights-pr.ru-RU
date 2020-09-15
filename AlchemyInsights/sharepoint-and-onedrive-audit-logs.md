---
title: Отчеты по классическим журналам аудита SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662221"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Журналы аудита SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Классические журналы аудита SharePoint

Прежний аудит SPO был перенесен в единый журнал аудита (UAL). Все устаревшие отчеты об аудите SPO теперь будут подаваться с помощью UAL, а устаревшие сигналы аудита будут перенесены на UAL.

Основные изменения:

* Фильтрация недоступна в качестве возможности.
* Выбор определенных событий для аудита недоступен. В [этом документе](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) приведен полный список событий аудита, доступных по умолчанию.
* Параметр **Расположение** в разделе **настроенные отчеты** недоступен.
* Параметр **Открытие или скачивание событий документов** недоступен.

[Настройка параметров аудита для семейства веб-сайтов](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Современные Объединенные журналы аудита SharePoint и OneDrive для обеспечения соответствия требованиям

* [Включение и выключение ведения журнала единого аудита](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

В SharePoint или OneDrive дополнительные настройки не требуются.

Используйте поиск в журнале аудита, чтобы проверить активность файлов, папок, пользователей, разрешений:

* [Действия, связанные с файлами и страницами](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Действия, связанные с папками](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Действия, связанные с общим доступом и запросами на доступ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Действия, связанные с синхронизацией](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Действия, связанные с администрированием сайта](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Дополнительные сведения о получении этих событий можно найти [в статье Поиск в журнале аудита](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
