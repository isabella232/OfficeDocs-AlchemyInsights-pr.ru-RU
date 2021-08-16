---
title: Микрозадержки или регулирование скорости в Exchange Online PowerShell
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
- "5106"
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098579"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Микрозадержки или регулирование скорости в Exchange Online PowerShell

При запуске сценариев и командлетов в Exchange Online могут отображаться предупреждения "Применена микрозадержка" или возникать задержки. Вот несколько советов по решению этой проблемы.

- Запустите наше средство диагностики, чтобы сделать политику регулирования PowerShell на вашем клиенте менее жесткой. Это решает проблему в большинстве случаев.
- Если проблема не исчезнет, попробуйте использовать [модуль PowerShell Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true): он включает командлеты на основе API REST, их производительность значительно выше. Это решение может быть оптимальным для множества часто используемых командлетов Get.
- Если нужно использовать командлеты, не входящие в состав модуля v2, см статью [Запуск командлетов PowerShell для большого количества пользователей в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). В ней описываются обходные решения для ограничений регулирования PowerShell в Exchange Online.
