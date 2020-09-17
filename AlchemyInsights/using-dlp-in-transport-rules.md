---
title: Использование защиты от потери данных в правилах транспорта
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
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773176"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="b3740-102">Использование защиты от потери данных в правилах транспорта</span><span class="sxs-lookup"><span data-stu-id="b3740-102">Using DLP in transport rules</span></span>

<span data-ttu-id="b3740-103">Чтобы интегрировать защиту от потери данных (DLP) в существующий транспорт, используйте условие "**Если сообщение содержит... Конфиденциальные сведения**" в параметрах правила транспорта.</span><span class="sxs-lookup"><span data-stu-id="b3740-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="b3740-104">**Дополнительные сведения:**</span><span class="sxs-lookup"><span data-stu-id="b3740-104">**For more details, see:**</span></span>

- <span data-ttu-id="b3740-105">Встроенные типы конфиденциальной информации DLP в правилах транспорта: [Интеграция правил конфиденциальной информации](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="b3740-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="b3740-106">Кроме того, вы можете проверить правило с тестированием или без тестирования политики с помощью режима тестирования для правила.</span><span class="sxs-lookup"><span data-stu-id="b3740-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="b3740-107">После создания правила нужно подождать 30 минут перед его тестированием.</span><span class="sxs-lookup"><span data-stu-id="b3740-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="b3740-108">См. раздел [Тестирование правил потока обработки почты/правил транспорта](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="b3740-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="b3740-109">**Примечание**. Если вы пытаетесь реализовать новую политику защиты от потери данных с правилами транспорта в Центре администрирования Exchange, используйте вместо этого раздел [Политики защиты от потери данных в Центре безопасности и соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b3740-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
