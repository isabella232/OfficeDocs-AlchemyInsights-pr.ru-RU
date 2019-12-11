---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959507"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6e7d1-102">Outlook не удается подключиться к общедоступным папкам</span><span class="sxs-lookup"><span data-stu-id="6e7d1-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6e7d1-103">Если доступ к общедоступным папкам не работает для нескольких пользователей, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="6e7d1-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="6e7d1-104">Подключитесь к EXO PowerShell и настройте DefaultPublicFolderMailbox учетной записи пользователя, чтобы она соотнесена с одной учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e7d1-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="6e7d1-105">Пример:</span><span class="sxs-lookup"><span data-stu-id="6e7d1-105">Example:</span></span>

<span data-ttu-id="6e7d1-106">Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс</span><span class="sxs-lookup"><span data-stu-id="6e7d1-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6e7d1-107">Set – Mailbox Проблемусер — значение \<DefaultPublicFolderMailbox из предыдущей команды></span><span class="sxs-lookup"><span data-stu-id="6e7d1-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6e7d1-108">Чтобы изменения вступили в силу, подождите хотя бы один час.</span><span class="sxs-lookup"><span data-stu-id="6e7d1-108">Wait at least one hour for the change to take effect.</span></span>