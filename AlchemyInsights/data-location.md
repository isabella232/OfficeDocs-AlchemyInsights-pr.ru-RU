---
title: Расположение данных
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627859"
---
# <a name="data-location"></a>Расположение данных

Вы можете просмотреть расположение клиента Office 365 в центре администрирования или подключиться к Exchange Online с помощью PowerShell.


**Центр администрирования:**
1. Выполните вход в [центр администрирования](https://admin.microsoft.com/Adminportal/Home).
2. Выберите **параметр** > **профиль организации**.
3. В разделе **расположение данных**выберите **Просмотреть сведения**.


**Типов**
1. Подключитесь к Exchange Online с помощью Windows PowerShell.
2. Выполните командлет [Get – OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) для отображения списка свойств клиента. 
3. Просмотрите свойство Организатионид.

Если у вас есть расположение данных для EXO и SPO, вы можете определить расположение данных для других служб, из которых можно использовать [данные](https://products.office.com/where-is-your-data-located).