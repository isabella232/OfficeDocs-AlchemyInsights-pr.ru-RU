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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038125"
---
# <a name="upn-sync-disabled"></a>Отключена синхронизация upN

Если вы начали синхронизацию с Azure AD до 30 марта 2016 г., запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое соответствие upN только для вашей организации:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Мягкий матч UPN автоматически включен для организаций, которые начали синхронизацию с Azure AD или после 30 марта 2016 г.
  
Дополнительные информацию о включаемом мягком совпадении в upN и других функций синхронизации см. в Подключение [службы синхронизации Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

