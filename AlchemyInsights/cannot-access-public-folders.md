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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891762"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="79c97-102">Outlook не удается подключиться к общедоступным папкам</span><span class="sxs-lookup"><span data-stu-id="79c97-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="79c97-103">Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="79c97-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="79c97-104">Подключитесь к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox учетной записи пользователя, чтобы он был сопоставлен с параметром рабочей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="79c97-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="79c97-105">Пример:</span><span class="sxs-lookup"><span data-stu-id="79c97-105">Example:</span></span>

<span data-ttu-id="79c97-106">Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс</span><span class="sxs-lookup"><span data-stu-id="79c97-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="79c97-107">Set – Mailbox Проблемусер — значение \<DefaultPublicFolderMailbox из предыдущей команды></span><span class="sxs-lookup"><span data-stu-id="79c97-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="79c97-108">Чтобы изменения вступили в силу, подождите хотя бы один час.</span><span class="sxs-lookup"><span data-stu-id="79c97-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="79c97-109">Если проблема не устранена, выполните указанные ниже [действия](https://aka.ms/pfcte) , чтобы устранить проблемы с доступом к общим папкам с помощью Outlook.</span><span class="sxs-lookup"><span data-stu-id="79c97-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>