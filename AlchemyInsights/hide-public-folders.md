---
title: Скрытие общедоступных папок
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294649"
---
# <a name="hide-public-folders"></a>Скрытие общедоступных папок

**Чтобы скрыть все дерево общедоступных папок**:

Следуйте инструкциям [этой](https://aka.ms/ControlPF) статьи, чтобы скрыть все дерево общедоступных папок для некоторых или всех пользователей.

**Чтобы скрыть определенную общедоступную папку**:

1. Добавление разрешений для пользователей, которым необходим доступ к общедоступной папке

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Удалите для пользователя разрешение **По умолчанию** из списка **разрешений**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
