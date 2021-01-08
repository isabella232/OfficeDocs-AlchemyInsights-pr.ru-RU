---
title: В центре безопасности получено сообщение о том, что подписки не найдены
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768528"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="4508b-102">В центре безопасности получено сообщение о том, что подписки не найдены</span><span class="sxs-lookup"><span data-stu-id="4508b-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="4508b-103">При доступе к центру безопасности Microsoft Defender появляется сообщение "не найдено подписок". Это означает, что служба Azure Active Directory (AAD), используемая для входа пользователя на портал, не имеет лицензии на Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="4508b-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="4508b-104">Лицензии Windows E5 и Office E5 - это две разные лицензии.</span><span class="sxs-lookup"><span data-stu-id="4508b-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="4508b-105">Если лицензия была приобретена, но не выделена для данного экземпляра AAD, откройте обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="4508b-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="4508b-106">Возможные варианты:</span><span class="sxs-lookup"><span data-stu-id="4508b-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="4508b-107">Возможная проблема при предоставлении лицензии.</span><span class="sxs-lookup"><span data-stu-id="4508b-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="4508b-108">По ошибке лицензия была предоставлена другому экземпляру Microsoft AAD, а не тому, который используется для проверки подлинности в службе.</span><span class="sxs-lookup"><span data-stu-id="4508b-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>