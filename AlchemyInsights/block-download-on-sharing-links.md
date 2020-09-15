---
title: Блокировать возможность скачивания по ссылкам совместного доступа
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685755"
---
# <a name="block-download-on-sharing-links"></a>Блокировать возможность скачивания по ссылкам совместного доступа

Параметр **«блокировать возможность скачивания»** доступен только для **ссылок, предназначенных только для просмотра** документов Office. При выборе этого параметра пользователи, получившие доступ к файлу с помощью созданной вами ссылки, не увидят параметры скачивания, печати и копирования файла.

Администраторы могут управлять тем, отображается ли параметр «блокировать возможность скачивания» только для файлов Office или нет, путем изменения `BlockDownloadLinksFileType` параметра в[командлетах Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) или [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
