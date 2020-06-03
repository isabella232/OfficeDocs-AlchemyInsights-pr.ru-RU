---
title: Устранение неполадок с советами по безопасности для проверок обнаружения мошенничества
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504996"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="30846-102">Устранение неполадок с советами по безопасности для проверок обнаружения мошенничества</span><span class="sxs-lookup"><span data-stu-id="30846-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="30846-103">Если вы получаете подсказку о безопасности с сообщением о том, что отправитель не прошел проверку на наличие мошенничества и может не являться тем, что они отображаются как ", то отправителю не удалось передать DKIM или проверки подлинности SPF.</span><span class="sxs-lookup"><span data-stu-id="30846-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="30846-104">Лучший способ решить эту проблему — отправителю выполнить самостоятельное авторизацию.</span><span class="sxs-lookup"><span data-stu-id="30846-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="30846-105">Если отправитель отправляет от вашего имени, вам потребуется авторизовать их, добавив IP-адрес отправителя в запись SPF.</span><span class="sxs-lookup"><span data-stu-id="30846-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="30846-106">[В статье Устранение неполадок, связанных с проверкой на наличие мошенничества,](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="30846-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="30846-107">Ниже приведены другие ссылки, которые могут помочь:</span><span class="sxs-lookup"><span data-stu-id="30846-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="30846-108">Как корпорация Майкрософт использует инфраструктуру политики отправителей (SPF) для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="30846-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="30846-109">Настройка SPF для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="30846-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
