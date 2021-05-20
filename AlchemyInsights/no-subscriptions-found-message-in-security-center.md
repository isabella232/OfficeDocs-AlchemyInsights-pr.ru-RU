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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544121"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="0533d-102">В центре безопасности получено сообщение о том, что подписки не найдены</span><span class="sxs-lookup"><span data-stu-id="0533d-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="0533d-103">При доступе к Центру безопасности в Microsoft Defender появляется сообщение "Подписки не найдены". Это означает, что служба Azure Active Directory (AAD), используемая для входа пользователя на портал, не имеет лицензии на ATP в Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="0533d-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="0533d-104">Лицензии Windows E5 и Office E5 — это две отдельные лицензии.</span><span class="sxs-lookup"><span data-stu-id="0533d-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="0533d-p101">Если лицензия была приобретена, но не подготовлена для данного экземпляра AAD, создайте запрос в службу поддержки. Возможные варианты:</span><span class="sxs-lookup"><span data-stu-id="0533d-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="0533d-107">Возможная проблема при предоставлении лицензии.</span><span class="sxs-lookup"><span data-stu-id="0533d-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="0533d-108">По ошибке лицензия была предоставлена другому экземпляру Microsoft AAD, а не тому, который используется для проверки подлинности в службе.</span><span class="sxs-lookup"><span data-stu-id="0533d-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>