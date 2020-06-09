---
title: 'Ошибка: правила на этом компьютере не совпадают'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618026"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="1537d-102">Ошибка: правила на этом компьютере не совпадают</span><span class="sxs-lookup"><span data-stu-id="1537d-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="1537d-103">Чтобы просмотреть обновленный статус этой известной проблемы, просмотрите [правила на этом компьютере не совпадают с правилами на сервере Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="1537d-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="1537d-104">Группа разработчиков Outlook реализовала исправление в сборке 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="1537d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="1537d-105">Исправление уже находится на странице "Предварительная работа" и будет переходить на ежемесячный канал в конце июня 2020.</span><span class="sxs-lookup"><span data-stu-id="1537d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="1537d-106">Если у вас есть фиксированная сборка, вы можете получить запрос "какие правила вы хотите сохранить" один раз в последний раз.</span><span class="sxs-lookup"><span data-stu-id="1537d-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="1537d-107">Нажмите кнопку сервер, когда появится соответствующий запрос, затем вернитесь в Outlook и повторно включите все отключенные правила.</span><span class="sxs-lookup"><span data-stu-id="1537d-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="1537d-108">Пока исправление не будет доступно, используйте следующее временное решение.</span><span class="sxs-lookup"><span data-stu-id="1537d-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="1537d-109">**Решение**: в последних отчетах возникла ошибка для тех, кто создал только правила клиентов в классической версии Outlook.</span><span class="sxs-lookup"><span data-stu-id="1537d-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="1537d-110">Если проблема не исчезнет, рассмотрите возможность удаления правил, а затем создание и изменение правил только в OWA (Outlook Web App), пока проблема не будет устранена.</span><span class="sxs-lookup"><span data-stu-id="1537d-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="1537d-111">Если не удается удалить правила вручную, вы можете выполнить команду Outlook при запуске Outlook, запустив Outlook. exe/клеанрулес.</span><span class="sxs-lookup"><span data-stu-id="1537d-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="1537d-112">Это приведет к удалению правил клиента и сервера.</span><span class="sxs-lookup"><span data-stu-id="1537d-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="1537d-113">Будут удалены все правила для всех учетных записей в профиле Outlook.</span><span class="sxs-lookup"><span data-stu-id="1537d-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="1537d-114">Эта команда далее задокументирована в статье параметры командной строки.</span><span class="sxs-lookup"><span data-stu-id="1537d-114">This command is further documented in the Command-line switches  article.</span></span>