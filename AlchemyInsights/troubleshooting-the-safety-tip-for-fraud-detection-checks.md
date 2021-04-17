---
title: Устранение неполадок в подсказке безопасности для проверки обнаружения мошенничества
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834744"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ac85f-102">Устранение неполадок в подсказке безопасности для проверки обнаружения мошенничества</span><span class="sxs-lookup"><span data-stu-id="ac85f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ac85f-103">Если вы получаете подсказку по безопасности с сообщением "Отправитель не справился с проверками обнаружения мошенничества и может не быть тем, кем они кажутся", то отправитель не прошел проверки подлинности DKIM или SPF.</span><span class="sxs-lookup"><span data-stu-id="ac85f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ac85f-104">Самый лучший способ для решения этой проблемы — авторизировать себя.</span><span class="sxs-lookup"><span data-stu-id="ac85f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ac85f-105">Если отправитель отправляет от вашего имени, необходимо авторизовать его, добавив IP-адрес отправитель в запись SPF.</span><span class="sxs-lookup"><span data-stu-id="ac85f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ac85f-106">Дополнительные сведения см. в дополнительных сведениях об устранении неполадок с красным [(подозрительным)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) советом по безопасности для проверки обнаружения мошенничества.</span><span class="sxs-lookup"><span data-stu-id="ac85f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ac85f-107">Вот некоторые другие ссылки, которые могут помочь:</span><span class="sxs-lookup"><span data-stu-id="ac85f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ac85f-108">Как Корпорация Майкрософт использует рамки политики отправитель (SPF) для предотвращения подмены</span><span class="sxs-lookup"><span data-stu-id="ac85f-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ac85f-109">Настройка SPF для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="ac85f-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
