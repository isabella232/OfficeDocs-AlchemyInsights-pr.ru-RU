---
title: Обновления Exchange Server безопасности
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449096"
---
# <a name="about-exchange-server-security-updates"></a>Обновления Exchange Server безопасности

Корпорация Майкрософт выпустила ряд критически важных обновлений безопасности для Exchange Server локальной службы. Затронутые версии серверов — это уровни обновления Exchange Server 2010, 2013, 2016 и 2019 годов. Exchange Online не влияет, но если у вас есть некоторые локально серверы Exchange из-за гибридной конфигурации, они потенциально уязвимы.

Для обновления локального сервера необходимо будет запускать по крайней мере следующие версии Exchange:

- Exchange 2010 Пакет обновления 3
- Exchange Server 2013 cu 23
- Exchange Server 2016 cu 19 или CU 18
- Exchange Server 2019 cu 8 или CU 7

См. в следующем объявлении о расположении исправлений: [Released: March 2021 Exchange Server обновления безопасности](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Важные примечания.**

Установка обновлений не будет работать, если на локальном сервере не запущены необходимые версии Exchange, как по вышеуказанном списку.

При установке обновлений вручную ознакомьтесь с разделом "Известные проблемы" обновления статей КБ для получения важных сведений. Обновления безопасности должны запускаться с повышенной подсказки CMD/PowerShell!
