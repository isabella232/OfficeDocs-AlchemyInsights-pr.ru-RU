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
description: При получении ошибки при активации Office 2013 г. в развертываниях служб удаленного рабочего стола (RDS) рассмотрите возможность включения ADAL путем редактирования реестра.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100775"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Ошибка при активации Office 2013 г. в службах удаленного рабочего стола

При получении ошибки при активации Office 2013 г. в развертываниях служб удаленного рабочего стола (RDS) рассмотрите возможность включения ADAL путем редактирования реестра.
  
|**Раздел реестра**|**Тип**|**Значение**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Дополнительные сведения см. в [рублях Enable Modern Authentication for Office 2013 на Windows устройствах.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL включен по умолчанию в Приложения Microsoft 365 для предприятий и Office 2016 г. Службы удаленного рабочего стола (RDS) ранее назывались службами терминалов.
  