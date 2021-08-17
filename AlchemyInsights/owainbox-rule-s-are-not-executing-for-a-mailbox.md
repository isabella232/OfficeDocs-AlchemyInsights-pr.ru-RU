---
title: 1332 OWA — правило "Входящие" не выполняется для почтового ящика
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040915"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило "Входящие" работает не так, как ожидалось

Проверка следующих параметров в Outlook в Интернете:

- Сообщение может быть перенаправлено, перенаправлено или ответило автоматически на основе правил входящие только один раз. Правило перенаправления (правило "Входящие" или правило потока почты, также известное как правило транспорта) может добавить в сообщение не более десяти получателей пересылания. Дополнительные сведения см. [в правилах "Журнал", "Транспорт" и "Входящие".](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Правила почтовых ящиков не работают на альтернативном почтовом ящике для журналов. Дополнительные сведения об альтернативном почтовом ящике для журналов см. в [журнале Alternate journaling mailbox.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Чтобы устранить эти проблемы, см. [в 2829319.](https://support.microsoft.com/kb/2829319)

Если предыдущие проблемы не применяются, запустите диагностический отчет по правилу "Входящие", прежде чем перенаправить проблему в службу поддержки Майкрософт:

1. Откройте почтовый ящик в Outlook в Интернете и нажмите кнопку <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Параметры**  >  **Просмотр всех Outlook Параметры**  >  **Почта**  >  **Правила**.

2. В нижней части страницы нажмите кнопку Если правила не работают, щелкните здесь, **чтобы создать диагностический отчет.**
