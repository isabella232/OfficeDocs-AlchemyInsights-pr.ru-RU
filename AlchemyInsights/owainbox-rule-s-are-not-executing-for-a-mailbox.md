---
title: '1332 Outlook: правила папки "Входящие" не выполняются для почтового ящика.'
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
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721604"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило для папки "Входящие" работает не так, как ожидалось

Проверьте следующие параметры в Outlook в Интернете:

- Сообщение может быть перенаправлено, переадресовано или отправлено автоматически на основе правил для папки "Входящие" только один раз. Правило перенаправления (правило транспорта или правило обработки почты), которое также называется правилом транспорта, может добавлять в сообщение не более десяти получателей пересылки. Для получения дополнительных сведений ознакомьтесь с разделом [журнала, транспорта и правил для папки "Входящие"](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правила для папки "Входящие" не работают в альтернативном почтовом ящике журналов. Дополнительные сведения о альтернативном почтовом ящике журналов можно узнать в разделе [альтернативный почтовый ящик журналов](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Чтобы устранить эти проблемы, ознакомьтесь со [статьей KB 2829319](https://support.microsoft.com/kb/2829319).

Если предыдущие проблемы не применяются, запустите диагностический отчет о правиле папки "Входящие" перед тем, как вы передаете ошибку в службу поддержки Майкрософт:

1. Откройте почтовый ящик в Outlook в Интернете и нажмите кнопку <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Параметры**  >  **Просмотр всех параметров Outlook**  >  **Mail (почта**  >  ) **Rules (правила**).

2. В нижней части страницы щелкните, **Если правила не работают, щелкните здесь, чтобы создать диагностический отчет**.
