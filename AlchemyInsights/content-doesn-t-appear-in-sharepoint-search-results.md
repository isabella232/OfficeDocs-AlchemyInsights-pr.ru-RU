---
title: Содержимое не появляется в SharePoint результатах поиска
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081623"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Содержимое не появляется в SharePoint результатах поиска

Выполните следующие действия по устранению неполадок, если ожидаемое содержимое не появится в результатах поиска:
  
1. Убедитесь, **что на** сайте, содержащем ожидаемое содержимое, установлено разрешение на просмотр контента в результатах поиска. Следуйте шагам [в содержимого Show на сайте в результатах поиска.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Убедитесь, **что в** списке или **библиотеке,** содержащем ожидаемое содержимое, установлено разрешение на просмотр контента в результатах поиска. Следуйте шагам в [шоу контента из списков или библиотек в результатах поиска.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Убедитесь, что макет страницы, документа или настраиваемой страницы опубликован в качестве **основной версии.** Следуйте шагу 3 в [Поиске не возвращает](https://go.microsoft.com/fwlink/?linkid=874525)все результаты в SharePoint Online .

4. Убедитесь, что у пользователя **есть разрешения** на просмотр контента. Следуйте шагам в [области понимания уровней](https://docs.microsoft.com/sharepoint/understanding-permission-levels)разрешений в SharePoint .
    
5. Если схема поиска была изменена путем добавления нового управляемого свойства, редактирования управляемого свойства или удаления управляемого свойства, потребуется запрос обхода и повторного индекса. **Переиндексировать** контент, следуя шагам в инструкции по обходу и повторной индексации сайта, библиотеки или [списка.](https://docs.microsoft.com/sharepoint/crawl-site-content) Это может занять некоторое время, подождите 24 часа, прежде чем снова проверить результаты.

Дополнительные сведения см. в [материалах Enable content on a site to be searchable.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
