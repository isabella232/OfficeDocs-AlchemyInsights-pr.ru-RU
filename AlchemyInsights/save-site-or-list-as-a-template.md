---
title: Сохранение сайта или списка в качестве шаблона
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770540"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="7f3ed-102">Сохранение сайта или списка в качестве шаблона</span><span class="sxs-lookup"><span data-stu-id="7f3ed-102">Save site or list as a template</span></span>

<span data-ttu-id="7f3ed-103">Шаблоны сайтов SharePoint — это готовые определения, разработанные с учетом определенных бизнес-потребностей.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="7f3ed-104">Дополнительные сведения см. [в статье Использование шаблонов для создания различных типов сайтов SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="7f3ed-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="7f3ed-105">Ниже приведены некоторые распространенные проблемы и решения относительно сохранения сайта или списка в качестве шаблона в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="7f3ed-106">**Кнопка "сохранить сайт/список шаблонов" недоступна или отсутствует**.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="7f3ed-107">Администраторам необходимо разрешить пользовательскому скрипту включить функции шаблона.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="7f3ed-108">Подробное описание действий, примеры и рекомендации [](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)см.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="7f3ed-109">Команда "сохранить сайт как шаблон" не поддерживается и может привести к ошибкам на сайтах, использующих инфраструктуру публикации SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="7f3ed-110">**Шаблон сайта не может быть создан или работает неправильно**</span><span class="sxs-lookup"><span data-stu-id="7f3ed-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="7f3ed-111">Возможно, шаблон не содержит [компонент](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не активируется.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="7f3ed-112">Если эта функция недоступна для активации в текущем семействе веб-сайтов, вы не можете использовать шаблон сайта для создания сайта.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="7f3ed-113">Убедитесь, что в списках или библиотеках превышено [ограничение числа элементов в представлении списка](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , равное 5000 элементов, так как это может заблокировать создание шаблона сайта.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="7f3ed-114">Возможно, на сайте используется слишком много ресурсов, поэтому шаблон сайта превышает ограничение в 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="7f3ed-115">Возникли проблемы с отображением данных из списка, в котором используется столбец подстановки.</span><span class="sxs-lookup"><span data-stu-id="7f3ed-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="7f3ed-116">Дополнительные сведения см. в разделе [созданный шаблоном список не отображает данные из соответствующего списка подстановки в SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="7f3ed-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="7f3ed-117">Более подробную информацию о распространенных проблемах и решениях можно найти в справочных материалах, [Создайте и используйте шаблоны сайтов](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="7f3ed-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

