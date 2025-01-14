---
title: Совместное использование с внешними пользователями не работает
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304382"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Устранение проблем SharePoint контента с внешними пользователями

Убедитесь, что внешний общий доступ включен для организации:
  
1. Перейдите на [страницу &amp; надстройки Services](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)в Центр администрирования Microsoft 365 и щелкните **Сайты**.
    
2. Убедитесь, что параметр включен в "Включен". Если выбрано "Только существующие внешние пользователи", убедитесь, что внешний пользователь указан в Центр администрирования Microsoft 365.
    
Убедитесь, что внешний общий доступ к сайту включен. Для классической коллекции сайтов:
  
1. В новом центре администрирования SharePoint в левой области щелкните **сайты**.
    
2. Выберите сайт или сайты, а на ленте щелкните **Раздел**.
    
Для сайта группы, который принадлежит Microsoft 365 группы, или сайта связи:
  
- Эти новые типы сайтов имеют тот же параметр общего доступа, что и для всей организации, если только в этом параметре для всей организации не разрешается делиться файлами с помощью ссылок, которые не требуют входов. В этом случае сайты позволяют обмениваться данными с новыми и существующими внешними пользователями, входивших в систему. Чтобы изменить параметр для определенных сайтов, используйте новый центр администрирования SharePoint Или PowerShell. [Подробнее](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Примечание.** Параметр внешнего обмена для любого сайта может быть более строгим, чем параметр всей организации, но не более допустимым, чем параметр всей организации. 
  

