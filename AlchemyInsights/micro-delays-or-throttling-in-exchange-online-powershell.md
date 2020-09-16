---
title: Микрозадержки или регулирование скорости в Exchange Online PowerShell
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
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743927"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Микрозадержки или регулирование скорости в Exchange Online PowerShell

При запуске сценариев и командлетов в Exchange Online могут отображаться предупреждения "Применена микрозадержка" или возникать задержки. Вот два предложения, связанные с этой проблемой:

- Попробуйте использовать [модуль PowerShell Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps): он включает командлеты на основе API REST, их производительность значительно выше. Это решение может быть оптимальным для множества часто используемых командлетов Get.
- Если нужно использовать командлеты, которые пока не входят в состав модуля v2, см статью [Запуск командлетов PowerShell для большого количества пользователей в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). В этой статье описываются обходные решения для возможных ограничений с регулированием скорости PowerShell в Exchange Online.
