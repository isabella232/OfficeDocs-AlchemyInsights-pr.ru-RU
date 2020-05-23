---
title: Решение проблем аутентификации SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264558"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="b35bc-102">Решение проблем аутентификации SMTP</span><span class="sxs-lookup"><span data-stu-id="b35bc-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="b35bc-103">Если вы получаете ошибки 5.7.57 или 5.7.3 при попытке отправки электронной почты SMTP и аутентификации с помощью клиента или приложения, необходимо проверить несколько вещей:</span><span class="sxs-lookup"><span data-stu-id="b35bc-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="b35bc-104">Аутентифицированная отправка SMTP может быть отключена в вашем клиенте или в почтовом ящике, который вы пытаетесь использовать (проверьте обе настройки).</span><span class="sxs-lookup"><span data-stu-id="b35bc-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="b35bc-105">Подробнее читайте в разделе [Включение или отключение отправки SMTP аутентифицированного клиента](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="b35bc-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="b35bc-106">Проверьте, включены ли [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для вашего клиента; если включено, SMTP-аутентификация с использованием базовой аутентификации (также известной как устаревшая; при этом будут использоваться имя пользователя и пароль) не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="b35bc-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
