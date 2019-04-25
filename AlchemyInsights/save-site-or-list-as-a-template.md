---
title: Сохранение сайта или списка в качестве шаблона
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243635"
---
# <a name="save-site-or-list-as-a-template"></a>Сохранение сайта или списка в качестве шаблона

Шаблоны сайтов SharePoint — это готовые определения, разработанные с учетом определенных бизнес-потребностей. Дополнительные сведения см. [в статье Использование шаблонов для создания различных типов сайтов SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Ниже приведены некоторые распространенные проблемы и решения относительно сохранения сайта или списка в качестве шаблона в SharePoint Online.

**Кнопка "сохранить сайт/список шаблонов" недоступна или отсутствует**. 

- Администраторам необходимо разрешить пользовательскому скрипту включить функции шаблона. Подробное описание действий, примеры и рекомендации [](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)см.


- Команда "сохранить сайт как шаблон" не поддерживается и может привести к ошибкам на сайтах, использующих инфраструктуру публикации SharePoint Server.


**Шаблон сайта не может быть создан или работает неправильно**

- Возможно, шаблон не содержит [компонент](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не активируется. Если эта функция недоступна для активации в текущем семействе веб-сайтов, вы не можете использовать шаблон сайта для создания сайта.


- Убедитесь, что в списках или библиотеках превышено [ограничение числа элементов в представлении списка](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , равное 5000 элементов, так как это может заблокировать создание шаблона сайта.


- Возможно, на сайте используется слишком много ресурсов, поэтому шаблон сайта превышает ограничение в 50 МБ.


- Возникли проблемы с отображением данных из списка, в котором используется столбец подстановки. Дополнительные сведения см. в разделе [созданный шаблоном список не отображает данные из соответствующего списка подстановки в SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Более подробную информацию о распространенных проблемах и решениях можно найти в справочных материалах, [Создайте и используйте шаблоны сайтов](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

