---
title: Устранение ошибки с кодом AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901630"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="409f3-102">Устранение ошибки с кодом AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="409f3-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="409f3-103">Чтобы устранить ошибку AADSTS50011, выполните рекомендуемое действие, описанное ниже.</span><span class="sxs-lookup"><span data-stu-id="409f3-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="409f3-104">**AADSTS50011**: InvalidReplyTo — адрес ответа отсутствует, неправильно настроен или не соответствует адресам ответа, настроенным для приложения.</span><span class="sxs-lookup"><span data-stu-id="409f3-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="409f3-105">В качестве решения добавьте этот отсутствующий адрес ответа в приложение Azure Active Directory (AD) или попросите сделать это пользователя с разрешениями на управление вашим приложением в AD.</span><span class="sxs-lookup"><span data-stu-id="409f3-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="409f3-106">Дополнительные сведения см. в статье по устранению ошибки [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span><span class="sxs-lookup"><span data-stu-id="409f3-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>