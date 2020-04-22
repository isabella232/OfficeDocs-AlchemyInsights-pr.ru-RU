---
title: Синхронизация имени участника-пользователя отключена
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726117"
---
# <a name="upn-sync-disabled"></a>Синхронизация имени участника-пользователя отключена

Если вы начали синхронизацию с Azure AD до 30 марта 2016, запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое обновление имени участника-пользователя только для вашей организации:
  
 **Set – Мсолдирсинкфеатуре — Feature Енаблесофтматчонупн — Enable $True**
  
Мягкое обновление UPN автоматически включается для организаций, которые начали синхронизироваться с Azure AD на или после 30 марта 2016 г.
  
Чтобы узнать больше о том, как включить мягкое сравнение на UPN и других функциях синхронизации, обратитесь к разделу [функции службы синхронизации Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

