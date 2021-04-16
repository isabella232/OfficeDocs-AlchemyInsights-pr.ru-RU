---
title: Exchange PowerShell и прекращение поддержки обычной проверки подлинности
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813485"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell и прекращение поддержки обычной проверки подлинности

Актуальные сведения о способе подключения к Exchange Online PowerShell без обычной проверки подлинности см. [здесь](https://aka.ms/exops-docs). Модуль PowerShell V2 не использует обычную проверку подлинности.

Обратите внимание, что на клиентском компьютере должна быть включена обычная проверка подлинности.
Новый модуль PowerShell версии 2 использует современную проверку подлинности с целью подключения для включения всех командлетов версии 2 на основе REST. В дополнение к командлетам версии 2 он также предоставляет вам доступ к более старым командлетам PowerShell (RPS), для которых требуется создание удаленного сеанса PowerShell. Создание сеанса RPS на компьютере с Windows требует включения службы WinRM BasicAuth на клиентском компьютере, даже если модуль использует механизм современной проверки подлинности для службы. Для передачи маркеров современной проверки подлинности используется конвейер обычной проверки подлинности WinRM. Если на клиентском компьютере отключена обычная проверка подлинности WinRM, новые командлеты версии 2 продолжат работать (но перестанут работать более старые командлеты RPS).
