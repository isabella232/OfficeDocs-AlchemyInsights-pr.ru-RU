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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655295"
---
# <a name="data-location"></a>Расположение данных

Вы можете просмотреть расположение клиента в центре администрирования или подключиться к Exchange Online с помощью PowerShell.


**Центр администрирования:**
1. Выполните вход в [центр администрирования](https://admin.microsoft.com/Adminportal/Home).
2. Выберите **параметр** > **профиль организации**.
3. В разделе **расположение данных**выберите **Просмотреть сведения**.


**Типов**
1. Подключитесь к Exchange Online с помощью Windows PowerShell.
2. Выполните командлет [Get – OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) для отображения списка свойств клиента. 
3. Просмотрите свойство Организатионид.

Если у вас есть расположение данных для EXO и SPO, вы можете определить расположение данных для других служб, из которых можно использовать [данные](https://products.office.com/where-is-your-data-located).