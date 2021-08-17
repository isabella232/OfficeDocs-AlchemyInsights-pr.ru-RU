---
title: Синхронизация профилей
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320722"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когда изменения профиля синхронизируются с SharePoint профилем пользователя?

SharePoint Для импорта пользователей и групп в приложение профилей пользователей в Интернете используется задание импортного времени Active Directory (AD Import). 
  
1. Импорт AD синхронизирует изменения из SharePoint магазина каталогов в приложение профилей пользователей. Эти изменения обрабатываются пакетами.
    
2. Задание timer выполняется до синхронизации изменений.
    
**Примечание.** Время, необходимое для запуска задания, зависит от количества изменений в процессе. Большое количество изменений занимает больше времени. В соглашении об уровне службы (SLA) говорится, что изменение пользователя в каталоге SharePoint online будет отражено в приложении профилей пользователей в течение 24 часов. 
  
[Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

