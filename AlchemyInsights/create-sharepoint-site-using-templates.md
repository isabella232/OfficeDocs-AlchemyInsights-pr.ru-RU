---
title: Создание сайта в SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770436"
---
# <a name="create-sharepoint-sites-using-templates"></a>Создание сайтов SharePoint с помощью шаблонов

Возможность сохранения сайта в виде шаблона не поддерживается с современными подключениями и сайтами групп. Более подробную информацию об использовании шаблонов можно узнать в статье [Сохранение, скачивание и отправка сайта SharePoint в качестве шаблона](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ниже приведены некоторые распространенные проблемы и решения относительно сохранения сайта или списка в качестве шаблона в SharePoint Online. 

**Кнопка "сохранить сайт/список шаблонов" недоступна или отсутствует**

Администраторам необходимо разрешить пользовательскому скрипту включить функции шаблона. Подробное описание действий, примеры и рекомендации см. 

- [Разрешение или запрещение пользовательских сценариев](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Команда "сохранить сайт как шаблон" не поддерживается и может привести к ошибкам на сайтах, использующих инфраструктуру публикации SharePoint Server.

**Шаблон сайта не может быть создан или работает неправильно**

Возможно, шаблон не содержит [компонент](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не активируется. Если эта функция недоступна для активации в текущем семействе веб-сайтов, вы не можете использовать шаблон сайта для создания сайта.

- Убедитесь, что в списках или библиотеках превышено [ограничение числа элементов в представлении списка](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , равное 5000 элементов, так как это может заблокировать создание шаблона сайта.

- Возможно, на сайте используется слишком много ресурсов, поэтому шаблон сайта превышает ограничение в 50 МБ.


- Возникли проблемы с отображением данных из списка, в котором используется столбец подстановки. Дополнительные сведения см. в разделе [созданный шаблоном список не отображает данные из соответствующего списка подстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Для получения более подробных сведений о распространенных проблемах и решениях проверьте [Создание и использование шаблонов сайтов](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



