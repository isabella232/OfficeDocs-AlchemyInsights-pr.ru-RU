---
title: Код ошибки 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709200"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Ошибка при активации Office 2013 в службах удаленных рабочих столов

Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.
  
|**Раздел реестра**|**Тип**|**Значение**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Дополнительную информацию можно узнать [в статье Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL включается по умолчанию в приложениях Microsoft 365 для предприятий и Office 2016. Службы удаленных рабочих столов (RDS) ранее назывались службами терминалов.
  