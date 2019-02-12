---
title: 1332 OWA - правил для папки «Входящие» не выполняются для почтового ящика
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915817"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="7194a-102">Правила папки «Входящие» не работает должным образом</span><span class="sxs-lookup"><span data-stu-id="7194a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="7194a-103">Проверьте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="7194a-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="7194a-p101">Сообщения могут быть перенаправлены, переадресованных или пересылаемых автоматически на основе правил папки "Входящие" только один раз. Перенаправление правило (правила папки "Входящие" или правило поток обработки почты, также известной как правила транспорта) можно добавить не более десяти переадресации получателей на сообщение. Дополнительные сведения см в [ограничения правил журнала, транспорта и папки «Входящие»](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="7194a-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="7194a-p102">Правила папки «Входящие» не работают на альтернативный почтовый ящик журналов. Дополнительные сведения о альтернативный почтовый ящик журналов можно [альтернативный почтовый ящик журналов](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="7194a-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="7194a-109">Чтобы исправить эти ошибки, обратитесь к разделу [2829319 КБ](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="7194a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="7194a-110">Если описанных ранее проблем, не применяются, запустите диагностического отчета правила папки «Входящие» перед перевести проблеме в службу поддержки Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="7194a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="7194a-111">Откройте почтовый ящик в Outlook в Интернете и щелкните **Параметры** \> **Параметры** \> **Упорядочить по электронной почте** \> **правила папки «Входящие»**.</span><span class="sxs-lookup"><span data-stu-id="7194a-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="7194a-112">В нижней части страницы нажмите кнопку **Если правила не работают, щелкните здесь для создания диагностического отчета**.</span><span class="sxs-lookup"><span data-stu-id="7194a-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

