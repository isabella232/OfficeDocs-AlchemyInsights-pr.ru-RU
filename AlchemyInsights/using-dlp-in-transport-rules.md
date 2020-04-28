---
title: Использование защиты от потери данных в правилах транспорта
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915301"
---
# <a name="using-dlp-in-transport-rules"></a>Использование защиты от потери данных в правилах транспорта

Чтобы интегрировать защиту от потери данных (DLP) в существующий транспорт, используйте условие "**Если сообщение содержит... Конфиденциальные сведения**" в параметрах правила транспорта.

**Дополнительные сведения:**

- Встроенные типы конфиденциальной информации DLP в правилах транспорта: [Интеграция правил конфиденциальной информации](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Кроме того, вы можете проверить правило с тестированием или без тестирования политики с помощью режима тестирования для правила.  После создания правила нужно подождать 30 минут перед его тестированием.

- См. раздел [Тестирование правил потока обработки почты/правил транспорта](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Примечание**. Если вы пытаетесь реализовать новую политику защиты от потери данных с правилами транспорта в Центре администрирования Exchange, используйте вместо этого раздел [Политики защиты от потери данных в Центре безопасности и соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
