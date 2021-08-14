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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923657"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когда изменения профиля синхронизируются с SharePoint профилем пользователя?

SharePoint Для импорта пользователей и групп в приложение профилей пользователей в Интернете используется задание импортного времени Active Directory (AD Import). 
  
1. Импорт AD синхронизирует изменения из SharePoint магазина каталогов в приложение профилей пользователей. Эти изменения обрабатываются пакетами.
    
2. Задание timer выполняется до синхронизации изменений.
    
> [!NOTE]
> Время, необходимое для запуска задания, зависит от количества изменений в процессе. Большое количество изменений занимает больше времени. В соглашении об уровне службы (SLA) говорится, что изменение пользователя в каталоге SharePoint online будет отражено в приложении профилей пользователей в течение 24 часов. 
  
[Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

