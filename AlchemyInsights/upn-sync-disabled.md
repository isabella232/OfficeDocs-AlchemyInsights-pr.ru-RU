---
title: Этот параметр отключен синхронизации имени участника-пользователя
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28309051"
---
# <a name="upn-sync-disabled"></a>Этот параметр отключен синхронизации имени участника-пользователя

Если запустить синхронизацию с Azure AD до 30 марта 2016, выполните следующий командлет Windows Azure AD PowerShell, чтобы включить соответствие программных имени участника-пользователя для вашей организации только:
  
 **SET-MsolDirSyncFeature-EnableSoftMatchOnUpn в функциях-включить $True**
  
Для организаций, которые удалось запустить синхронизацию с Azure AD не ранее 30 марта 2016 включается автоматически программных совпадение имени участника-пользователя.
  
Для получения дополнительных сведений о включении программных совпадение на имя участника-пользователя и другие функции синхронизации, можно найти [компонентов службы синхронизации Azure AD подключение](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

