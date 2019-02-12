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
description: Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929102"
---
<span data-ttu-id="4c59b-103">Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="4c59b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="4c59b-104">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="4c59b-104">**Registry key**</span></span>|<span data-ttu-id="4c59b-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="4c59b-105">**Type**</span></span>|<span data-ttu-id="4c59b-106">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4c59b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4c59b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4c59b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4c59b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4c59b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4c59b-109">1</span><span class="sxs-lookup"><span data-stu-id="4c59b-109">1</span></span>  <br/> |
   
<span data-ttu-id="4c59b-110">Дополнительные сведения можно [Включить современных проверки подлинности для Office 2013 на устройствах Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4c59b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4c59b-p101">ADAL включен по умолчанию в Office 365 профессиональный плюс и Office 2016. > служб удаленных рабочих столов (RDS) прежнее название служб терминалов.</span><span class="sxs-lookup"><span data-stu-id="4c59b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

