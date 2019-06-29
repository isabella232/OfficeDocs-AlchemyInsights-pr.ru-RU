---
title: Контент не отображается в результатах поиска SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363831"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Контент не отображается в результатах поиска SharePoint

Выполните следующие действия по устранению неполадок, когда ожидаемое содержимое не отображается в результатах поиска:
  
1. Убедитесь, что **сайт** , который содержит ожидаемый контент, настроен на разрешение отображения контента в результатах поиска. Выполните действия, описанные в разделе [Просмотр контента сайта в результатах поиска](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Убедитесь, что **список** или **Библиотека** , содержащие ожидаемый контент, настроены на разрешение отображения контента в результатах поиска. Выполните действия, описанные в статье [Показать содержимое из списков или библиотек в результатах поиска](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Убедитесь, что страница, документ или пользовательский макет страницы опубликованы в качестве **основной версии.** Выполните шаг 3 в разделе [Поиск не возвращает все результаты в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Убедитесь, что у пользователя есть **разрешения** на просмотр контента. Выполните действия, описанные в статье [Общие сведения о уровнях разрешений в SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Если схема поиска была изменена путем добавления нового управляемого свойства, редактирования управляемого свойства или удаления управляемого свойства, потребуется выполнить обход контента и повторное индексирование. **Выполните повторную индексацию** контента, выполнив действия, описанные в статье [Ручное сканирование и повторная индексация сайта, библиотеки или списка](https://docs.microsoft.com/sharepoint/crawl-site-content). Это может занять некоторое время, подождите 24 часа, прежде чем снова будет проверять результаты.

Дополнительные сведения можно найти в статье [Включение поддержки поиска контента на сайте](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
