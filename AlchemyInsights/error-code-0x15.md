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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499395"
---
<span data-ttu-id="e1a5f-103">Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="e1a5f-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="e1a5f-104">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="e1a5f-104">**Registry key**</span></span>|<span data-ttu-id="e1a5f-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="e1a5f-105">**Type**</span></span>|<span data-ttu-id="e1a5f-106">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e1a5f-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e1a5f-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="e1a5f-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="e1a5f-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="e1a5f-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="e1a5f-109">^1</span><span class="sxs-lookup"><span data-stu-id="e1a5f-109">1</span></span>  <br/> |
   
<span data-ttu-id="e1a5f-110">Дополнительные сведения можно [Включить современных проверки подлинности для Office 2013 на устройствах Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="e1a5f-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e1a5f-p101">ADAL включен по умолчанию в Office 365 профессиональный плюс и Office 2016. > служб удаленных рабочих столов (RDS) прежнее название служб терминалов.</span><span class="sxs-lookup"><span data-stu-id="e1a5f-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

