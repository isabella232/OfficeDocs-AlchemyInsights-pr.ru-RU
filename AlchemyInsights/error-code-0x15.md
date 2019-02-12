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
Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра. 
  
|**Раздел реестра**|**Тип**|**Значение**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Дополнительные сведения можно [Включить современных проверки подлинности для Office 2013 на устройствах Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL включен по умолчанию в Office 365 профессиональный плюс и Office 2016. > служб удаленных рабочих столов (RDS) прежнее название служб терминалов. 
  

