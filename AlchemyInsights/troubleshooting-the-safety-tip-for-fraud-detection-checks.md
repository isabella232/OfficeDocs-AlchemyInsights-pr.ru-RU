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
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533216"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="e2c6e-102">Устранение неполадок с советами по безопасности для проверок обнаружения мошенничества</span><span class="sxs-lookup"><span data-stu-id="e2c6e-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="e2c6e-103">Если вы получаете подсказку о безопасности с сообщением о том, что отправитель не прошел проверку на наличие мошенничества и может не являться тем, что они отображаются как ", то отправителю не удалось передать DKIM или проверки подлинности SPF.</span><span class="sxs-lookup"><span data-stu-id="e2c6e-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="e2c6e-104">Лучший способ решить эту проблему — отправителю выполнить самостоятельное авторизацию.</span><span class="sxs-lookup"><span data-stu-id="e2c6e-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="e2c6e-105">Если отправитель отправляет от вашего имени, вам потребуется авторизовать их, добавив IP-адрес отправителя в запись SPF.</span><span class="sxs-lookup"><span data-stu-id="e2c6e-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="e2c6e-106">[В статье Устранение неполадок, связанных с проверкой на наличие мошенничества,](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="e2c6e-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="e2c6e-107">Ниже приведены другие ссылки, которые могут помочь:</span><span class="sxs-lookup"><span data-stu-id="e2c6e-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="e2c6e-108">Как Office 365 использует инфраструктуру политики отправителей (SPF) для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="e2c6e-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="e2c6e-109">Настройка SPF в Office 365 для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="e2c6e-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
