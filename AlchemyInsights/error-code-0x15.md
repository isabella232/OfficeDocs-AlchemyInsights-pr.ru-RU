---
title: Код ошибки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308506"
---
<span data-ttu-id="6f11b-103">Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="6f11b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="6f11b-104">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="6f11b-104">**Registry key**</span></span>|<span data-ttu-id="6f11b-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="6f11b-105">**Type**</span></span>|<span data-ttu-id="6f11b-106">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6f11b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6f11b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="6f11b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="6f11b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="6f11b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="6f11b-109">1</span><span class="sxs-lookup"><span data-stu-id="6f11b-109">1</span></span>  <br/> |
   
<span data-ttu-id="6f11b-110">Дополнительные сведения можно [Включить современных проверки подлинности для Office 2013 на устройствах Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="6f11b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="6f11b-p101">ADAL включен по умолчанию в Office 365 профессиональный плюс и Office 2016. > Удаленных рабочих столов (RDS) прежнее название служб терминалов.</span><span class="sxs-lookup"><span data-stu-id="6f11b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

