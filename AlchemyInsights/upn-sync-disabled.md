---
title: Отключена синхронизация upN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782164"
---
# <a name="upn-sync-disabled"></a>Отключена синхронизация upN

Если вы начали синхронизацию с Azure AD до 30 марта 2016 г., запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое соответствие upN только для вашей организации:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Мягкий матч UPN автоматически включен для организаций, которые начали синхронизацию с Azure AD или после 30 марта 2016 г.
  
Дополнительные информацию о включении мягкого совпадения в upN и других функций синхронизации см. в дополнительных подробностях службы синхронизации [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

