---
title: Не удалось добавить рабочий процесс утверждения 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748697"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="02e7c-102">Не удалось добавить рабочий процесс утверждения 2010</span><span class="sxs-lookup"><span data-stu-id="02e7c-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="02e7c-103">В семействе веб-сайтов Microsoft SharePoint невозможно добавить глобальный рабочий процесс для повторного использования (например, "утверждение-SharePoint 2010") в список или библиотеку.</span><span class="sxs-lookup"><span data-stu-id="02e7c-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="02e7c-104">Чтобы устранить эту проблему, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="02e7c-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="02e7c-105">Откройте корневой веб-сайт семейства веб-сайтов в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="02e7c-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="02e7c-106">В разделе **объекты сайта**выберите **рабочие процессы**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="02e7c-107">В разделе **создать** на ленте **рабочие процессы** выберите **Рабочий процесс для повторного использования**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="02e7c-108">В форме **Создание рабочего процесса для повторного использования** введите имя \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="02e7c-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="02e7c-109">В качестве **типа платформы**выберите элемент **рабочий процесс SharePoint 2010**и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="02e7c-110">В разделе **Сохранение** ленты **рабочего процесса** нажмите кнопку **опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="02e7c-111">В разделе **Управление** ленты **рабочего процесса** выберите параметр **опубликовать глобально**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="02e7c-112">В появившемся диалоговом окне подтверждения нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="02e7c-113">В веб-браузере найдите корневой веб-сайт семейства веб-сайтов, а затем доступ к \> **функциям семейства веб**-сайтов с помощью **параметров сайта** .</span><span class="sxs-lookup"><span data-stu-id="02e7c-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="02e7c-114">Переключать функции **рабочих процессов** :</span><span class="sxs-lookup"><span data-stu-id="02e7c-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="02e7c-115">· Если компонент *активирован* , щелкните **Отключить,** а затем нажмите кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="02e7c-116">· Если компонент *отключен, нажмите* кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="02e7c-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="02e7c-117">Для получения дополнительных сведений обратитесь к следующей [статье](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="02e7c-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

