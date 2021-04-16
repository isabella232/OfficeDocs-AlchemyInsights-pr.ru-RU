---
title: Ошибка. Правила на этом компьютере не совпадают
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782965"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="0453d-102">Ошибка. Правила на этом компьютере не совпадают</span><span class="sxs-lookup"><span data-stu-id="0453d-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="0453d-103">Чтобы увидеть обновленный статус этой известной проблемы, см. в рублях Правила на этом компьютере не соответствуют правилам [Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="0453d-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="0453d-104">Группа Outlook реализовала исправление в сборке 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="0453d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="0453d-105">Исправление уже на сайте Insider Fast и будет переходить на Ежемесячный канал в конце июня 2020 г.</span><span class="sxs-lookup"><span data-stu-id="0453d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="0453d-106">После фиксированной сборки вы можете получить подсказку "Какие правила вы хотите сохранить" в последний раз.</span><span class="sxs-lookup"><span data-stu-id="0453d-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="0453d-107">Выберите Сервер при запросе, а затем возвращайся в Outlook и включив все отключенные правила.</span><span class="sxs-lookup"><span data-stu-id="0453d-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="0453d-108">До тех пор, пока исправление не будет доступно, воспользуйтесь следующим обходным решением:</span><span class="sxs-lookup"><span data-stu-id="0453d-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="0453d-109">**Обходное решение.** В последних отчетах проблема возникла только для тех, кто создал клиентские правила на рабочем столе Outlook.</span><span class="sxs-lookup"><span data-stu-id="0453d-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="0453d-110">Если вы продолжаете работать с проблемой, рассмотрите возможность удаления правил и создания и редактирования правил только в OWA (Outlook Web App), пока проблема не будет решена.</span><span class="sxs-lookup"><span data-stu-id="0453d-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="0453d-111">Если вы не можете удалить правила вручную, вы можете запустить команду Outlook при запуске Outlook, Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="0453d-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="0453d-112">Это позволит удалить как клиентские, так и серверные правила.</span><span class="sxs-lookup"><span data-stu-id="0453d-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="0453d-113">Он удалит все правила для всех учетных записей в профиле Outlook.</span><span class="sxs-lookup"><span data-stu-id="0453d-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="0453d-114">Далее эта команда описана в статье Коммутаторы командной строки.</span><span class="sxs-lookup"><span data-stu-id="0453d-114">This command is further documented in the Command-line switches article.</span></span>

