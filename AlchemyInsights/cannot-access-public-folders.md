---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891762"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не удается подключиться к общедоступным папкам

Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте выполнить следующие действия:

Подключитесь к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox учетной записи пользователя, чтобы он был сопоставлен с параметром рабочей учетной записи пользователя.

Пример:

Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс

Set – Mailbox Проблемусер — значение \<DefaultPublicFolderMailbox из предыдущей команды>

Чтобы изменения вступили в силу, подождите хотя бы один час.

Если проблема не устранена, выполните указанные ниже [действия](https://aka.ms/pfcte) , чтобы устранить проблемы с доступом к общим папкам с помощью Outlook.