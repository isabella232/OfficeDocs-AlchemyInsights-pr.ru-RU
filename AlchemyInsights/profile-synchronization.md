---
title: Синхронизация профилей
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768126"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когда изменения профиля синхронизируются с приложением профиля пользователя SharePoint?

SharePoint Online использует задание таймера импорта Active Directory (импорт AD) для импорта пользователей и групп в приложение профилей пользователей. 
  
1. Служба импорта Active Directory синхронизирует изменения из хранилища каталогов SharePoint Online с приложением профилей пользователей. Эти изменения обрабатываются в пакетах.
    
2. Задание таймера выполняется до тех пор, пока изменения не будут синхронизированы.
    
> [!NOTE]
> Время, необходимое для выполнения задания, зависит от количества изменений, которые необходимо обработать. Большое количество изменений занимает больше времени. Соглашение об уровне обслуживания (SLA) указывает на то, что изменение пользователя в каталоге SharePoint Online будет отражено в приложении профиля пользователя в течение 24 часов. 
  
[Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

