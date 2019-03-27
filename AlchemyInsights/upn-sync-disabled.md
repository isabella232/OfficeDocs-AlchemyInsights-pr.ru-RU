---
title: Синхронизация имени участника-пользователя отключена
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767256"
---
# <a name="upn-sync-disabled"></a>Синхронизация имени участника-пользователя отключена

Если вы начали синхронизацию с Azure AD до 30 марта 2016, запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое обновление имени участника-пользователя только для вашей организации:
  
 **Set – Мсолдирсинкфеатуре — Feature Енаблесофтматчонупн — Enable $True**
  
Мягкое обновление UPN автоматически включается для организаций, которые начали синхронизироваться с Azure AD на или после 30 марта 2016 г.
  
Чтобы узнать больше о том, как включить мягкое сравнение на UPN и других функциях синхронизации, обратитесь к разделу [функции службы синхронизации Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

