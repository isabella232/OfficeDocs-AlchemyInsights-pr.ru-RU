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
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801782"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когда изменения профиля синхронизируются с приложением профиля пользователя SharePoint?

SharePoint Online использует задание таймера импорта Active Directory (импорт AD) для импорта пользователей и групп в приложение профилей пользователей. 
  
1. Служба импорта Active Directory синхронизирует изменения из хранилища каталогов SharePoint Online с приложением профилей пользователей. Эти изменения обрабатываются в пакетах.
    
2. Задание таймера выполняется до тех пор, пока изменения не будут синхронизированы.
    
> [!NOTE]
> Время, необходимое для выполнения задания, зависит от количества изменений, которые необходимо обработать. Большое количество изменений занимает больше времени. Соглашение об уровне обслуживания (SLA) указывает на то, что изменение пользователя в каталоге SharePoint Online будет отражено в приложении профиля пользователя в течение 24 часов. 
  
[Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

