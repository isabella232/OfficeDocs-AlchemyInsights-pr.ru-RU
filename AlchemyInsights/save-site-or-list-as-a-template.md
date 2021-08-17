---
title: Сохранение сайта или списка в качестве шаблона
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109217"
---
# <a name="save-site-or-list-as-a-template"></a>Сохранение сайта или списка в качестве шаблона

Шаблоны сайтов SharePoint — это готовые определения, разработанные с учетом определенных бизнес-потребностей. Дополнительные сведения см. в [веб-сайте Использование шаблонов для создания](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)различных SharePoint сайтов.

Вот некоторые распространенные проблемы и решения, касающиеся сохранения сайта или списка в качестве шаблона SharePoint Online.

**Сохранить кнопку шаблона сайта или списка недоступна или отсутствует.** 

- Для включения компонентов шаблона администраторам необходимо разрешить пользовательский сценарий. Подробные действия, примеры и соображения см. в [примере Разрешить или предотвратить настраиваемый сценарий.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Команда "Сохранить сайт как шаблон" не поддерживается и может привести к проблемам на сайтах, использующих инфраструктуру публикации SharePoint Server.


**Шаблон сайта не может быть создан или не работает правильно**

- Шаблон может пропустить [функцию и](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активироваться. Если функция недоступна для активации в текущем семействе веб-сайтов, вы не сможете использовать шаблон для создания сайта.


- Проверьте, не превышено ли для какого-то списка или библиотеки [пороговое значение представления списка](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) (5000 элементов), так как это может препятствовать созданию шаблона сайта.


- Сайт может использовать слишком много ресурсов, поэтому шаблон сайта превышает 50 мегабайт (МБ).


- Существуют проблемы с отображением данных из списка, содержащего столбец подстановок. Дополнительные сведения см. в [списке шаблонов,](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)в который не отображаются данные из правильного списка SharePoint Online.


Дополнительные сведения о распространенных проблемах и решениях можно получить в справочной ссылке, в этой области [можно найти шаблоны](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)сайтов и использовать их.

