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
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="b21b5-102">Создание сайтов SharePoint с помощью шаблонов</span><span class="sxs-lookup"><span data-stu-id="b21b5-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="b21b5-103">Возможность сохранения сайта в виде шаблона не поддерживается с современными подключениями и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="b21b5-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="b21b5-104">Более подробную информацию об использовании шаблонов можно узнать в статье [Сохранение, скачивание и отправка сайта SharePoint в качестве шаблона](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="b21b5-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="b21b5-105">Ниже приведены некоторые распространенные проблемы и решения относительно сохранения сайта или списка в качестве шаблона в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b21b5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="b21b5-106">**Кнопка "сохранить сайт/список шаблонов" недоступна или отсутствует**</span><span class="sxs-lookup"><span data-stu-id="b21b5-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="b21b5-107">Администраторам необходимо разрешить пользовательскому скрипту включить функции шаблона.</span><span class="sxs-lookup"><span data-stu-id="b21b5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="b21b5-108">Подробное описание действий, примеры и рекомендации см.</span><span class="sxs-lookup"><span data-stu-id="b21b5-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="b21b5-109">Разрешение или запрещение пользовательских сценариев</span><span class="sxs-lookup"><span data-stu-id="b21b5-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="b21b5-110">Команда "сохранить сайт как шаблон" не поддерживается и может привести к ошибкам на сайтах, использующих инфраструктуру публикации SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="b21b5-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="b21b5-111">**Шаблон сайта не может быть создан или работает неправильно**</span><span class="sxs-lookup"><span data-stu-id="b21b5-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="b21b5-112">Возможно, шаблон не содержит [компонент](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не активируется.</span><span class="sxs-lookup"><span data-stu-id="b21b5-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="b21b5-113">Если эта функция недоступна для активации в текущем семействе веб-сайтов, вы не можете использовать шаблон сайта для создания сайта.</span><span class="sxs-lookup"><span data-stu-id="b21b5-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="b21b5-114">Убедитесь, что в списках или библиотеках превышено [ограничение числа элементов в представлении списка](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , равное 5000 элементов, так как это может заблокировать создание шаблона сайта.</span><span class="sxs-lookup"><span data-stu-id="b21b5-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="b21b5-115">Возможно, на сайте используется слишком много ресурсов, поэтому шаблон сайта превышает ограничение в 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="b21b5-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="b21b5-116">Возникли проблемы с отображением данных из списка, в котором используется столбец подстановки.</span><span class="sxs-lookup"><span data-stu-id="b21b5-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="b21b5-117">Дополнительные сведения см. в разделе [созданный шаблоном список не отображает данные из соответствующего списка подстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="b21b5-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="b21b5-118">Для получения более подробных сведений о распространенных проблемах и решениях проверьте [Создание и использование шаблонов сайтов](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="b21b5-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



