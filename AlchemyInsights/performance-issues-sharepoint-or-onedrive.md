---
title: Проблемы с производительностью- SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911855"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive, недоступны или недоступны для нескольких пользователей

SharePoint или OneDrive может быть медленным, недоступным или недоступным, или может отображать службу недоступной или 503 ошибки, по нескольким причинам:
  
- Если ваш SharePoint или OneDrive для нескольких пользователей медленный или отложенный, может возникнуть временная проблема с обслуживанием, когда пользователи испытывают периодические задержки или ошибки навигации при доступе к SharePoint сайтам или OneDrive контенту. Проверьте [панель мониторинга работоспособности служб](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), чтобы узнать, затронута ли ваша организация.
  
- Пользователи могут получить *503* сервер занят ошибкой при попытке перейти к SharePoint или OneDrive сайтов. Эта ошибка может быть вызвана регулированием в SharePoint службы. для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования. Регулирование ограничивает количество действий пользователя или одновременных звонков (по сценарию или коду), чтобы предотвратить чрезмерное использование ресурсов. Дополнительные сведения о регулирование см. в этой информации, избегайте регулирования или блокировки в [SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Если вы испытываете медленную  производительность на классическом или [](https://aka.ms/perftool) современном SharePoint сайте или странице, используйте средство диагностики страниц для анализа страниц. 
  
- Если вы по-прежнему испытываете общую медленную производительность, просмотрите ресурсы в нижней части этой статьи: Введение в настройку [производительности для SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  