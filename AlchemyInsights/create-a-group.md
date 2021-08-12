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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929318"
---
# <a name="create-a-group"></a>Создание группы

В этом разделе описывается создание групп.

**Разрешение на создание группы**

Убедитесь, что вы уполномочены создавать новую группу. Глобальные администраторы могут отключить создание групп на портале Azure или панели доступа. Может потребоваться администратор для создания новой группы или для получения соответствующих разрешений.

**Управление разрешениями на создание групп**

1. Глобальные администраторы могут управлять разрешениями на создание групп (по соображениям безопасности) или группами Office 365, созданными на портале Azure или панели доступа, выбрав параметры "Пользователи могут создавать группы безопасности на порталах Azure" или "Пользователи могут создавать группы Office 365 в порталах Azure" во всех группах Общего  >  **(Параметры)**.
2. Вы также можете ограничить создание группы, чтобы выбрать группу пользователей, если у вас есть Azure Active Directory P1 Premium лицензии.

**Отключение приветствия для Office 365 участников группы**

Приветствие, отправленное пользователям, добавленным в Office 365 группы, может быть отключено путем установки **ЕдинойGroupWelcomeMessageEnabled** для False в Powershell. Подробные сведения об этом параметре см. [здесь](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

