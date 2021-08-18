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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316699"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Ошибка при активации Office 2013 г. в службах удаленного рабочего стола

При получении ошибки при активации Office 2013 г. в развертываниях служб удаленного рабочего стола (RDS) рассмотрите возможность включения ADAL путем редактирования реестра.
  
|**Раздел реестра**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Дополнительные сведения см. в [рублях Enable Modern Authentication for Office 2013 на Windows устройствах.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Примечание.** ADAL включен по умолчанию в Приложения Microsoft 365 для предприятий и Office 2016 г. Службы удаленного рабочего стола (RDS) ранее назывались службами терминалов.
  