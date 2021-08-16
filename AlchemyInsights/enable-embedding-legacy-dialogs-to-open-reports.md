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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003402"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешение внедрения устаревших диалоговых окон для открытия отчетов

**Симптом**

Пользователям не удается открыть отчеты. "Возникла проблема. Подробности см. в технических сведениях".

**Причина**

Отчеты не загружаются в UCI с ошибкой "Дескриптор формы имеет значение null или не определен". Отчетам в UCI по-прежнему требуются устаревшие диалоговые окна, поэтому в системе пользователя должен быть включен параметр *allowlegacydialogsembedding*.

**Решение**

1. Выберите **Параметры >Администрирование > Параметры системы > вкладка "Общее"**.

2. Присвойте параметру "Разрешить внедрение некоторых устаревших диалогов в браузерный клиент с единым интерфейсом" значение **Да**.
