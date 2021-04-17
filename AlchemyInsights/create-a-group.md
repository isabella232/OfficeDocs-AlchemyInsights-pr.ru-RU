---
title: Создание группы
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816373"
---
# <a name="create-a-group"></a>Создание группы

В этом разделе описывается создание групп.

**Разрешение на создание группы**

Убедитесь, что вы уполномочены создавать новую группу. Глобальные администраторы могут отключить создание групп на портале Azure или панели доступа. Может потребоваться администратор для создания новой группы или для получения соответствующих разрешений.

**Управление разрешениями на создание групп**

1. Глобальные администраторы могут управлять разрешениями на создание групп (по соображениям безопасности) или группами Office 365, созданными на портале Azure или панели доступа, выбрав параметры "Пользователи могут создавать группы безопасности на порталах Azure" или "Пользователи могут создавать группы Office 365 в порталах Azure" во всех группах Общего  >  **(Параметры)**.
2. Вы также можете ограничить создание группы, чтобы выбрать группу пользователей, если у вас есть лицензия Azure Active Directory P1 Premium.

**Отключение приветствия для новых членов группы Office 365**

Приветствие, отправленное пользователям, добавленным в группы Office 365, может быть отключено путем установки **ЕдинойGroupWelcomeMessageEnabled** для False в Powershell. Подробные сведения об этом параметре см. [здесь](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

