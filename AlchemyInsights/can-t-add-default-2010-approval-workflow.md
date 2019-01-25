---
title: Не удается добавить по умолчанию рабочий процесс утверждения 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485997"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="65770-102">Не удается добавить по умолчанию рабочий процесс утверждения 2010</span><span class="sxs-lookup"><span data-stu-id="65770-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="65770-103">В семействе сайтов Microsoft SharePoint нельзя добавить к списку или библиотеке глобального рабочего процесса (например, «утверждение – SharePoint 2010»).</span><span class="sxs-lookup"><span data-stu-id="65770-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="65770-104">Чтобы устранить эту проблему, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="65770-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="65770-105">Откройте корневой веб-сайт семейства веб-сайтов в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="65770-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="65770-106">В списке **Объекты сайта**выберите **рабочие процессы**.</span><span class="sxs-lookup"><span data-stu-id="65770-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="65770-107">В разделе **Создать** на ленте **рабочие процессы** выберите **Рабочий процесс для повторного использования**.</span><span class="sxs-lookup"><span data-stu-id="65770-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="65770-p101">**Создание рабочего процесса для повторного использования** формы введите имя \* \*\*Repair2010\*\*\*. **Тип платформы**выберите **Рабочий процесс SharePoint 2010**и нажмите кнопку « **ОК»**.</span><span class="sxs-lookup"><span data-stu-id="65770-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="65770-110">В разделе **Сохранить** на ленте **рабочего процесса** выберите **Опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="65770-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="65770-p102">В разделе **Управление** на ленте **рабочего процесса** выберите **Опубликовать в глобальном уровне**. В диалоговом окне подтверждения нажмите **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="65770-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="65770-p103">В веб-браузере, найдите корневой веб-сайт семейства веб-сайтов и затем доступ к **Параметрам сайта** \> **Возможности семейства сайтов**. Затем включения и отключения компонента **рабочих процессов** :</span><span class="sxs-lookup"><span data-stu-id="65770-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="65770-115">· Если компонент *активирован* , нажмите кнопку **Отключить** и нажмите кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="65770-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="65770-116">· Если компонент *отключено* , нажмите кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="65770-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="65770-117">Для получения дополнительных сведений обратитесь к следующей [статье](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="65770-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

