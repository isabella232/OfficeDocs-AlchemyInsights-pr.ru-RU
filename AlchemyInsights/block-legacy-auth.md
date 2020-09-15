---
title: блокклегациаус
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685611"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="8be5e-102">Блокировка устаревшей проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8be5e-102">Blocking legacy authentication</span></span>

<span data-ttu-id="8be5e-103">Традиционная аутентификация — это термин, обозначающий запрос на проверку подлинности, который делают:</span><span class="sxs-lookup"><span data-stu-id="8be5e-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="8be5e-104">Старые клиенты Office, которые не используют современные проверки подлинности (например, Office 2010 Client).</span><span class="sxs-lookup"><span data-stu-id="8be5e-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="8be5e-105">Любые клиенты, использующие устаревшие почтовые протоколы, например IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="8be5e-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="8be5e-106">Для получения дополнительных сведений об блокировании устаревшей проверки подлинности и включении современного режима проверки [подлинности см.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="8be5e-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="8be5e-107">Параметры безопасности по умолчанию в Azure Active Directory (Azure AD) упрощают защиту и защиту Организации.</span><span class="sxs-lookup"><span data-stu-id="8be5e-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="8be5e-108">Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности для распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="8be5e-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="8be5e-109">Дополнительные сведения о значениях по умолчанию для системы безопасности приведены в разделе [что такое параметры безопасности по умолчанию?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="8be5e-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="8be5e-110">**Примечание**. Если ваш клиент был создан или после октября 22nd, 2019, возможно, вы столкнулись с новым поведением по умолчанию, а в клиенте уже включены параметры безопасности по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8be5e-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="8be5e-111">В целях защиты всех наших пользователей по умолчанию выполняется развертывание всех новых клиентов.</span><span class="sxs-lookup"><span data-stu-id="8be5e-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
