---
title: Код ошибки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388258"
---
<span data-ttu-id="4c97b-103">Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.</span><span class="sxs-lookup"><span data-stu-id="4c97b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4c97b-104">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="4c97b-104">**Registry key**</span></span>|<span data-ttu-id="4c97b-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="4c97b-105">**Type**</span></span>|<span data-ttu-id="4c97b-106">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4c97b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4c97b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4c97b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4c97b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4c97b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4c97b-109">1,1</span><span class="sxs-lookup"><span data-stu-id="4c97b-109">1</span></span>  <br/> |

<span data-ttu-id="4c97b-110">Дополнительную информацию можно узнать [в статье Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4c97b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4c97b-111">ADAL включается по умолчанию в Office 365 профессиональный плюс и Office 2016.</span><span class="sxs-lookup"><span data-stu-id="4c97b-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4c97b-112">Службы удаленных рабочих столов (RDS) > ранее назывались службами терминалов.</span><span class="sxs-lookup"><span data-stu-id="4c97b-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  