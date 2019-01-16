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
Если ошибка при активации Office 2013 на развертывание служб удаленных рабочих столов (RDS), можно включить ADAL с помощью реестра. 
  
|**Раздел реестра**|**Тип**|**Значение**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Дополнительные сведения можно [Включить современных проверки подлинности для Office 2013 на устройствах Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL включен по умолчанию в Office 365 профессиональный плюс и Office 2016. > Удаленных рабочих столов (RDS) прежнее название служб терминалов. 
  

