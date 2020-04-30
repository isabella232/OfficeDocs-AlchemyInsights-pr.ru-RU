---
title: Микрозадержки или регулирование скорости в Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947901"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Микрозадержки или регулирование скорости в Exchange Online PowerShell

При запуске сценариев и командлетов в Exchange Online могут отображаться предупреждения "Применена микрозадержка" или возникать задержки. Вот два предложения, связанные с этой проблемой:

- Попробуйте использовать [модуль PowerShell Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps): он включает командлеты на основе API REST, их производительность значительно выше. Это решение может быть оптимальным для множества часто используемых командлетов Get.
- Если нужно использовать командлеты, которые пока не входят в состав модуля v2, см статью [Запуск командлетов PowerShell для большого количества пользователей в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). В этой статье описываются обходные решения для возможных ограничений с регулированием скорости PowerShell в Exchange Online.
