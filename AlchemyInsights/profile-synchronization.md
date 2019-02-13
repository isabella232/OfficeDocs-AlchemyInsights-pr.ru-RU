---
title: Синхронизация профилей
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920101"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когда изменения профиля синхронизации для приложения профилей пользователей SharePoint?

SharePoint Online с помощью задания таймера Импорт Active Directory (AD Import) для импорта пользователей и групп в приложение профилей пользователей. 
  
1. AD Import синхронизирует изменения из хранилища каталогов SharePoint Online для приложения профилей пользователей. Эти изменения обрабатываются пакетами.
    
2. Задание таймера выполняется до синхронизации изменений.
    
> [!NOTE]
> Время, необходимое для запуска задания зависит от числа изменения для обработки. Большое число изменений занимает больше времени. Соглашение об уровне службы (SLA) указано, что изменение пользователя в каталоге SharePoint Online будет отображаться в приложение профилей пользователей в течение 24 часов. 
  
[Дополнительные сведения о синхронизации профилей пользователей в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

