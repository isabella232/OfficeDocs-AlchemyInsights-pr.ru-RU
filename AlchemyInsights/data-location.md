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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207274"
---
# <a name="data-location"></a>Расположение данных

Вы можете просмотреть расположение клиента Office 365 в центре администрирования или подключиться к Exchange Online с помощью PowerShell.


**Центр администрирования:**
1. Выполните вход в [центр администрирования](https://admin.microsoft.com/Adminportal/Home).
2. Выберите **параметр** > **профиль организации**.
3. В разделе **расположение данных**выберите **Просмотреть сведения**.


**Типов**
1. Подключитесь к Exchange Online с помощью Windows PowerShell.
2. Выполните командлет [Get – OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) для отображения списка свойств клиента. 
3. Просмотрите свойство Организатионид.

Если у вас есть расположение данных для EXO и SPO, вы можете определить расположение данных для других служб, из которых можно использовать [данные](https://products.office.com/where-is-your-data-located).