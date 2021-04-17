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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818049"
---
# <a name="changing-ews-throttling-settings"></a>Изменение параметров регулирования EWS

Запустите автоматизированный тест, который позволит вам изменить политику регулирования EWS на весь период миграции. Обратите внимание: даже если он запущен, объем импорта EWS по-прежнему будет ограничен 150 МБ в 5 мин на почтовый ящик; для повышения скорости одновременно выполняйте миграцию большего количества пользователей.

Обратите внимание, что изменения политики регулирования не действуют со следующими типами миграции (с помощью средств Microsoft): гибридная, прямая или поэтапная (RPC/HTTP), IMAP, G Suite, общедоступная папка или служба импорта PST-файлов.