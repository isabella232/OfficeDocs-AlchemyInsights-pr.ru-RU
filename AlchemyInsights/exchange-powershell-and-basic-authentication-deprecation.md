---
title: Exchange PowerShell и прекращение поддержки обычной проверки подлинности
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
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782988"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell и прекращение поддержки обычной проверки подлинности

Актуальные сведения о способе подключения к Exchange Online PowerShell без обычной проверки подлинности см. [здесь](https://aka.ms/exops-docs). Модуль PowerShell V2 не использует обычную проверку подлинности.

Обратите внимание, что на клиентском компьютере должна быть включена обычная проверка подлинности.
Новый модуль PowerShell версии 2 использует современную проверку подлинности с целью подключения для включения всех командлетов версии 2 на основе REST. В дополнение к командлетам версии 2 он также предоставляет вам доступ к более старым командлетам PowerShell (RPS), для которых требуется создание удаленного сеанса PowerShell. Создание сеанса RPS на компьютере с Windows требует включения службы WinRM BasicAuth на клиентском компьютере, даже если модуль использует механизм современной проверки подлинности для службы. Для передачи маркеров современной проверки подлинности используется конвейер обычной проверки подлинности WinRM. Если на клиентском компьютере отключена обычная проверка подлинности WinRM, новые командлеты версии 2 продолжат работать (но перестанут работать более старые командлеты RPS).
