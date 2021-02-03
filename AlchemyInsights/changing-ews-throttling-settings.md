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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="163c0-102">Изменение параметров регулирования EWS</span><span class="sxs-lookup"><span data-stu-id="163c0-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="163c0-103">Запустите автоматизированный тест, который позволит вам изменить политику регулирования EWS на весь период миграции.</span><span class="sxs-lookup"><span data-stu-id="163c0-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="163c0-104">Обратите внимание: даже если он запущен, объем импорта EWS по-прежнему будет ограничен 150 МБ в 5 мин на почтовый ящик; для повышения скорости одновременно выполняйте миграцию большего количества пользователей.</span><span class="sxs-lookup"><span data-stu-id="163c0-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="163c0-105">Обратите внимание, что изменения политики регулирования не действуют со следующими типами миграции (с помощью средств Microsoft): гибридная, прямая или поэтапная (RPC/HTTP), IMAP, G Suite, общедоступная папка или служба импорта PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="163c0-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>