---
title: Разрешение внедрения устаревших диалоговых окон для открытия отчетов
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
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806448"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешение внедрения устаревших диалоговых окон для открытия отчетов

**Симптом**

Пользователям не удается открыть отчеты. "Возникла проблема. Подробности см. в технических сведениях".

**Причина**

Отчеты не загружаются в UCI с ошибкой "Дескриптор формы имеет значение null или не определен". Отчетам в UCI по-прежнему требуются устаревшие диалоговые окна, поэтому в системе пользователя должен быть включен параметр *allowlegacydialogsembedding*.

**Решение**

1. Выберите **Параметры >Администрирование > Параметры системы > вкладка "Общее"**.

2. Присвойте параметру "Разрешить внедрение некоторых устаревших диалогов в браузерный клиент с единым интерфейсом" значение **Да**.
