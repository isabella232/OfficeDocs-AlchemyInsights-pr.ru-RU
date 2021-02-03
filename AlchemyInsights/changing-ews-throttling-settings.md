---
title: Изменение параметров регулирования EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075910"
---
# <a name="changing-ews-throttling-settings"></a>Изменение параметров регулирования EWS

Запустите автоматизированный тест, который позволит вам изменить политику регулирования EWS на весь период миграции. Обратите внимание: даже если он запущен, объем импорта EWS по-прежнему будет ограничен 150 МБ в 5 мин на почтовый ящик; для повышения скорости одновременно выполняйте миграцию большего количества пользователей.

Обратите внимание, что изменения политики регулирования не действуют со следующими типами миграции (с помощью средств Microsoft): гибридная, прямая или поэтапная (RPC/HTTP), IMAP, G Suite, общедоступная папка или служба импорта PST-файлов.