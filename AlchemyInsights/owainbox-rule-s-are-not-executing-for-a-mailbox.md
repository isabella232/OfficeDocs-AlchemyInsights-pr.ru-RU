---
title: '1332 Outlook: правила папки "Входящие" не выполняются для почтового ящика.'
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858757"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="73017-102">Правило для папки "Входящие" работает не так, как ожидалось</span><span class="sxs-lookup"><span data-stu-id="73017-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="73017-103">Проверьте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="73017-103">Verify the following settings:</span></span>

- <span data-ttu-id="73017-104">Сообщение может быть перенаправлено, переадресовано или отправлено автоматически на основе правил для папки "Входящие" только один раз.</span><span class="sxs-lookup"><span data-stu-id="73017-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="73017-105">Правило перенаправления (правило транспорта или правило обработки почты), которое также называется правилом транспорта, может добавлять в сообщение не более десяти получателей пересылки.</span><span class="sxs-lookup"><span data-stu-id="73017-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="73017-106">Для получения дополнительных сведений ознакомьтесь с разделом [журнала, транспорта и правил для папки "Входящие"](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="73017-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="73017-107">Правила для папки "Входящие" не работают в альтернативном почтовом ящике журналов.</span><span class="sxs-lookup"><span data-stu-id="73017-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="73017-108">Дополнительные сведения о альтернативном почтовом ящике журналов можно узнать в разделе [альтернативный почтовый ящик журналов](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="73017-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="73017-109">Чтобы устранить эти проблемы, ознакомьтесь со [статьЕй KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="73017-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="73017-110">Если предыдущие проблемы не применяются, запустите диагностический отчет о правиле папки "Входящие" перед тем, как вы передаете ошибку в службу поддержки Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="73017-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="73017-111">Откройте почтовый ящик в Outlook в Интернете и выберите **Параметры** \> **настройки** \> **Упорядочить** \> **правила для папки "Входящие"**.</span><span class="sxs-lookup"><span data-stu-id="73017-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="73017-112">В нижней части страницы щелкните, **Если правила не работают, щелкните здесь, чтобы создать диагностический отчет**.</span><span class="sxs-lookup"><span data-stu-id="73017-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
