---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068428"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Медленный, недоступный или недоступный для нескольких пользователей SharePoint или OneDrive

SharePoint или OneDrive может быть медленной, недоступен или недоступен или может отображать недоступные службы или 503 ошибок, по нескольким причинам:
  
- Если сайт SharePoint или OneDrive работает медленнее или задержано для нескольких пользователей, может возникнуть временная ошибка службы, из-за которой при доступе пользователей к сайтам SharePoint или контенту в OneDrive возникают временные задержки или ошибки навигации. Просмотрите [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить, влияет ли ваша организация на работу.
  
- При попытке перейти к сайтам SharePoint или OneDrive пользователи могут получить сообщение о *занятости сервера 503* . Эта ошибка может быть вызвана регулированием в службе SharePoint. для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования. Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов. Для получения дополнительных сведений об регулированиях см. [Избегайте регулирования или блокировки в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- При низкой производительности с помощью **классического** или **современного** сайта или страницы SharePoint используйте [средство диагностики страниц](https://aka.ms/perftool) для анализа страниц.
  
- Если вы по-прежнему работает с низкой производительностью, ознакомьтесь с ресурсами в нижней части этой статьи: " [Введение в настройку производительности для SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334) ".
  