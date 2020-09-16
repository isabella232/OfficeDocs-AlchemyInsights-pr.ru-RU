---
title: Синхронизация имени участника-пользователя отключена
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749527"
---
# <a name="upn-sync-disabled"></a>Синхронизация имени участника-пользователя отключена

Если вы начали синхронизацию с Azure AD до 30 марта 2016, запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое обновление имени участника-пользователя только для вашей организации:
  
 **Set – Мсолдирсинкфеатуре — Feature Енаблесофтматчонупн — Enable $True**
  
Мягкое обновление UPN автоматически включается для организаций, которые начали синхронизироваться с Azure AD на или после 30 марта 2016 г.
  
Чтобы узнать больше о том, как включить мягкое сравнение на UPN и других функциях синхронизации, обратитесь к разделу [функции службы синхронизации Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

