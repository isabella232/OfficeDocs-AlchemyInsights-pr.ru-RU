---
title: Изменение параметров регулирования EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968390"
---
# <a name="changing-ews-throttling-settings"></a>Изменение параметров регулирования EWS

Запустите автоматизированный тест, который позволит вам изменить политику регулирования EWS на весь период миграции. Обратите внимание: даже если он запущен, объем импорта EWS по-прежнему будет ограничен 150 МБ в 5 мин на почтовый ящик; для повышения скорости одновременно выполняйте миграцию большего количества пользователей.

Обратите внимание, что изменения политики регулирования не действуют со следующими типами миграции (с помощью средств Microsoft): гибридная, прямая или поэтапная (RPC/HTTP), IMAP, G Suite, общедоступная папка или служба импорта PST-файлов.