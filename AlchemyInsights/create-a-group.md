---
title: Создание группы
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086393"
---
# <a name="create-a-group"></a>Создание группы

В этом разделе описывается создание групп.

**Разрешение на создание группы**

Убедитесь, что у вас есть разрешение на создание новой группы. Глобальные администраторы могут отключить создание групп на портале или панели доступа Azure. Возможно, вам потребуется администратор, чтобы создать новую группу или предоставить вам соответствующие разрешения.

**Управление разрешениями на создание групп**

1. Глобальные администраторы могут управлять разрешениями на создание групп (по причинам, связанным с безопасностью) или группами Office 365, созданными на портале или панели доступа Azure, выбрав "пользователи могут создавать группы безопасности в порталах Azure" или "пользователи могут создавать группы Office 365 в порталах Azure" во **всех группах**  >  **Общие (параметры)**.
2. Вы также можете ограничить создание групп, чтобы выбрать группу пользователей, если у вас есть лицензия Azure Active Directory P1 Premium.

**Отключение уведомления приветствия для новых участников группы Office 365**

Уведомление о приглашении, отправленное пользователям, добавленным в группы Office 365, можно отключить, задав для **UnifiedGroupWelcomeMessageEnabled** значение false в PowerShell. В этой [статье](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)рассказывается о данном параметре.

