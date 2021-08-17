---
title: Создание сайта в SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057979"
---
# <a name="create-sharepoint-sites-using-templates"></a>Создание SharePoint сайтов с использованием шаблонов

Возможность сохранить сайт как шаблон не поддерживается для современных информационных сайтов и сайтов групп. Дополнительные сведения об использовании шаблонов сайтов см. в статье [Сохранение, загрузка и передача сайта SharePoint в качестве шаблона](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Вот некоторые распространенные проблемы и решения, касающиеся сохранения сайта или списка в качестве шаблона в Sharepoint Online. 

**Сохранить кнопку шаблона сайта/списка недоступна или отсутствует**

Для включения компонентов шаблона администраторам необходимо разрешить пользовательский сценарий. Подробные действия, примеры и соображения см. в 

- [Разрешение и запрещение пользовательского сценария](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Команда "Сохранить сайт как шаблон" не поддерживается и может привести к проблемам на сайтах, использующих инфраструктуру публикации SharePoint Server.

**Шаблон сайта не может быть создан или не работает правильно**

Шаблон может пропустить [функцию и](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активироваться. Если функция недоступна для активации в текущем семействе веб-сайтов, вы не сможете использовать шаблон для создания сайта.

- Проверьте, не превышено ли для какого-то списка или библиотеки [пороговое значение представления списка](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) (5000 элементов), так как это может препятствовать созданию шаблона сайта.

- Возможно, сайт использует слишком много ресурсов, поэтому размер шаблона сайта превышает ограничение 50 МБ.


- Существуют проблемы с отображением данных из списка, содержащего столбец подстановок. Дополнительные сведения см. в статье [В списке, созданном с помощью шаблона, не отображаются данные из правильного списка подстановок в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Дополнительные сведения об общих проблемах и решениях можно найти в [create and use site templates.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



