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
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="1b014-102">Использование защиты от потери данных в правилах транспорта</span><span class="sxs-lookup"><span data-stu-id="1b014-102">Using DLP in transport rules</span></span>

<span data-ttu-id="1b014-103">Чтобы интегрировать защиту от потери данных (DLP) в существующий транспорт, используйте условие "**Если сообщение содержит... Конфиденциальные сведения**" в параметрах правила транспорта.</span><span class="sxs-lookup"><span data-stu-id="1b014-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="1b014-104">**Дополнительные сведения:**</span><span class="sxs-lookup"><span data-stu-id="1b014-104">**For more details, see:**</span></span>

- <span data-ttu-id="1b014-105">Встроенные типы конфиденциальной информации DLP в правилах транспорта: [Интеграция правил конфиденциальной информации](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="1b014-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="1b014-106">Кроме того, вы можете проверить правило с тестированием или без тестирования политики с помощью режима тестирования для правила.</span><span class="sxs-lookup"><span data-stu-id="1b014-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="1b014-107">После создания правила нужно подождать 30 минут перед его тестированием.</span><span class="sxs-lookup"><span data-stu-id="1b014-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="1b014-108">См. раздел [Тестирование правил потока обработки почты/правил транспорта](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="1b014-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="1b014-109">**Примечание**. Если вы пытаетесь реализовать новую политику защиты от потери данных с правилами транспорта в Центре администрирования Exchange, используйте вместо этого раздел [Политики защиты от потери данных в Центре безопасности и соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1b014-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
