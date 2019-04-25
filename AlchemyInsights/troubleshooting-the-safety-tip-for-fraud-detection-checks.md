---
title: Устранение неполадок с советами по безопасности для проверок обнаружения мошенничества
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391222"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="3296e-102">Устранение неполадок с советами по безопасности для проверок обнаружения мошенничества</span><span class="sxs-lookup"><span data-stu-id="3296e-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="3296e-103">Если вы получаете подсказку о безопасности с сообщением о том, что отправитель не прошел проверку на наличие мошенничества и может не являться тем, что они отображаются как ", то отправителю не удалось передать DKIM или проверки подлинности SPF.</span><span class="sxs-lookup"><span data-stu-id="3296e-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="3296e-104">Лучший способ решить эту проблему — отправителю выполнить самостоятельное авторизацию.</span><span class="sxs-lookup"><span data-stu-id="3296e-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="3296e-105">Если отправитель отправляет от вашего имени, вам потребуется авторизовать их, добавив IP-адрес отправителя в запись SPF.</span><span class="sxs-lookup"><span data-stu-id="3296e-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="3296e-106">[В статье устраненИе неполадок, связанных с проверкой на наличие мошенничества,](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="3296e-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="3296e-107">Ниже приведены другие ссылки, которые могут помочь:</span><span class="sxs-lookup"><span data-stu-id="3296e-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="3296e-108">Как Office 365 использует инфраструктуру политики отправителей (SPF) для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="3296e-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="3296e-109">Настройка SPF в Office 365 для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="3296e-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

