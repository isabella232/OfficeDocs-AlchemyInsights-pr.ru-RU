---
title: Разрешение внедрения устаревших диалоговых окон для открытия отчетов
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814277"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешение внедрения устаревших диалоговых окон для открытия отчетов

**Симптом**

Пользователям не удается открыть отчеты. "Возникла проблема. Подробности см. в технических сведениях".

**Причина**

Отчеты не загружаются в UCI с ошибкой "Дескриптор формы имеет значение null или не определен". Отчетам в UCI по-прежнему требуются устаревшие диалоговые окна, поэтому в системе пользователя должен быть включен параметр *allowlegacydialogsembedding*.

**Решение**

1. Выберите **Параметры >Администрирование > Параметры системы > вкладка "Общее"**.

2. Присвойте параметру "Разрешить внедрение некоторых устаревших диалогов в браузерный клиент с единым интерфейсом" значение **Да**.
