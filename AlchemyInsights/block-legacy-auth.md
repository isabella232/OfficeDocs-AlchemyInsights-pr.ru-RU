---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820191"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="b781a-102">Блокировка устаревшей проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b781a-102">Blocking legacy authentication</span></span>

<span data-ttu-id="b781a-103">Традиционная аутентификация — это термин, обозначающий запрос на проверку подлинности, который делают:</span><span class="sxs-lookup"><span data-stu-id="b781a-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="b781a-104">Старые клиенты Office, которые не используют современную проверку подлинности (например, клиент Office 2010).</span><span class="sxs-lookup"><span data-stu-id="b781a-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="b781a-105">Любые клиенты, использующие устаревшие почтовые протоколы, например IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="b781a-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="b781a-106">Дополнительные сведения о блокировке устаревшей проверки подлинности и в том, что касается включения современной проверки подлинности, обратитесь к [блокированию устаревшей проверки подлинности.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="b781a-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="b781a-107">По умолчанию безопасность в Azure Active Directory (Azure AD) упрощает безопасность и помогает защитить организацию.</span><span class="sxs-lookup"><span data-stu-id="b781a-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="b781a-108">По умолчанию в безопасности содержатся преднастройные параметры безопасности для распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="b781a-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="b781a-109">Дополнительные сведения о дефолтах безопасности можно найти в этой [ссылке.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="b781a-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="b781a-110">**Примечание.** Если клиент был создан 22 октября 2019 г. или после него, возможно, вы столкнулись с новым поведением по умолчанию и уже включили в клиенте по умолчанию безопасность.</span><span class="sxs-lookup"><span data-stu-id="b781a-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="b781a-111">Чтобы защитить всех пользователей, для всех созданных новых клиентов в настоящее время выкатываются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b781a-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
