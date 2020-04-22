---
title: Не удалось активировать отсутствующий рабочий процесс
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762114"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="7a92e-102">Не удалось активировать отсутствующий рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="7a92e-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="7a92e-103">В семействе веб-сайтов Microsoft SharePoint невозможно добавить глобальный рабочий процесс для повторного использования (например, "утверждение-SharePoint 2010") в список или библиотеку.</span><span class="sxs-lookup"><span data-stu-id="7a92e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7a92e-104">Чтобы устранить эту проблему, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="7a92e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7a92e-105">Откройте корневой веб-сайт семейства веб-сайтов в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="7a92e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7a92e-106">В разделе **объекты сайта**выберите **рабочие процессы**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7a92e-107">В разделе **создать** на ленте **рабочие процессы** выберите **Рабочий процесс для повторного использования**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7a92e-108">В форме **Создание рабочего процесса для повторного использования** введите имя \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="7a92e-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7a92e-109">В качестве **типа платформы**выберите элемент **рабочий процесс SharePoint 2010**и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7a92e-110">В разделе **Сохранение** ленты **рабочего процесса** нажмите кнопку **опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7a92e-111">В разделе **Управление** ленты **рабочего процесса** выберите параметр **опубликовать глобально**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7a92e-112">В появившемся диалоговом окне подтверждения нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7a92e-113">В веб-браузере найдите корневой веб-сайт семейства веб-сайтов, а затем доступ к \> **функциям семейства веб**-сайтов с помощью **параметров сайта** .</span><span class="sxs-lookup"><span data-stu-id="7a92e-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7a92e-114">Затем переключите компонент **рабочих процессов** :</span><span class="sxs-lookup"><span data-stu-id="7a92e-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7a92e-115">· Если компонент *активирован* , щелкните **Отключить,** а затем нажмите кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7a92e-116">· Если компонент *отключен, нажмите* кнопку **активировать**.</span><span class="sxs-lookup"><span data-stu-id="7a92e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7a92e-117">Для получения дополнительных сведений обратитесь к следующей [статье](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7a92e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

