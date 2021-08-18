---
title: Teams не запускается
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329339"
---
# <a name="teams-doesnt-launch"></a>Teams не запускается

Если вы пытаетесь открыть Microsoft Teams, но он никогда не запускается, попробуйте выполнить следующие действия:

1. Перейдите в **%appdata%\Microsoft\Teams**.
1. Удалите содержимое папки.
1. Перезагрузите компьютер и попробуйте запустить Teams.

Возможно, вам необходимо переустановить Teams. Чтобы переустановить:

1. Удалите Teams с помощью панели управления.
1. Перейдите в **%appdata%\Microsoft\Teams\Application Cache**.
1. Удалите содержимое папки.
1. Перейдите в **%appdata%\Microsoft\teams\Cache**.
1. Удалите содержимое папки.
1. Перезагрузите компьютер, а затем скачайте и установите Teams.

Если вы хотите запустить диагностику в клиенте для определенного пользователя, который не может войти, начните новый поиск с ключевым словом **TeamsUserUnableToSignIn** и следуйте советам.