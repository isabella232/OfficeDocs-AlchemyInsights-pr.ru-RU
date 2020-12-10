---
title: 'Устранение неполадок голосовой почты '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608008"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="6b361-102">Устранение неполадок голосовой почты</span><span class="sxs-lookup"><span data-stu-id="6b361-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="6b361-103">Убедитесь, что функция "занято при занятости" является преднамеренной.</span><span class="sxs-lookup"><span data-stu-id="6b361-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="6b361-104">Если эта функция не требуется для этого пользователя:</span><span class="sxs-lookup"><span data-stu-id="6b361-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="6b361-105">Перейдите в [центр администрирования Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="6b361-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="6b361-106">На левой границе Навигация по политикам **голосовых**  >  **вызовов**  >  **управляет** политиками в **политике вызовов**.</span><span class="sxs-lookup"><span data-stu-id="6b361-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="6b361-107">Выберите **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="6b361-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="6b361-108">Выполните поиск пользователя и измените политику вызовов на ту, которая **занята в занятии, доступна при** **отключении**.</span><span class="sxs-lookup"><span data-stu-id="6b361-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="6b361-109">Нажмите **Применить**.</span><span class="sxs-lookup"><span data-stu-id="6b361-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="6b361-110">Репликация изменений в политиках может занять до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="6b361-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="6b361-111">Дополнительные сведения об этой функции: " [занято на занятии" доступно в вызове](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="6b361-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
