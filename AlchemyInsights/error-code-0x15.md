---
title: Код ошибки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402752"
---
<span data-ttu-id="353cd-103">Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.</span><span class="sxs-lookup"><span data-stu-id="353cd-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="353cd-104">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="353cd-104">**Registry key**</span></span>|<span data-ttu-id="353cd-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="353cd-105">**Type**</span></span>|<span data-ttu-id="353cd-106">**Значение**</span><span class="sxs-lookup"><span data-stu-id="353cd-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="353cd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="353cd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="353cd-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="353cd-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="353cd-109">1 </span><span class="sxs-lookup"><span data-stu-id="353cd-109">1</span></span>  <br/> |
   
<span data-ttu-id="353cd-110">Дополнительную информацию можно узнать [в статье Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="353cd-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="353cd-111">ADAL включается по умолчанию в Office 365 профессиональный плюс и Office 2016.</span><span class="sxs-lookup"><span data-stu-id="353cd-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="353cd-112">Службы удаленных рабочих столов _Гт_ (RDS) ранее назывались службами терминалов.</span><span class="sxs-lookup"><span data-stu-id="353cd-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

