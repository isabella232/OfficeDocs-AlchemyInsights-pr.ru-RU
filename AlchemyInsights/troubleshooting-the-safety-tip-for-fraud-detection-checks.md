---
title: Устранение неполадок системы безопасности совет по мошенничества проверяет
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308847"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="be069-102">Устранение неполадок системы безопасности совет по мошенничества проверяет</span><span class="sxs-lookup"><span data-stu-id="be069-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="be069-p101">Если вы являетесь начало подсказку безопасности, который говорит «отправитель не удалось наших проверок обнаружения мошенничества и могут быть пользователей, которые они», а затем отправитель не прошел ПРОВЕРКУ или SPF проверку подлинности. — Это лучший способ решения этой проблемы для отправителя для авторизации сами. Если отправитель отправляет от вашего имени, необходимо авторизовать их путем добавления IP-адрес отправителя для записи SPF.</span><span class="sxs-lookup"><span data-stu-id="be069-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="be069-106">В разделе [Устранение неполадок красного (подозрительные) безопасности совет по мошенничества проверяет](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) Дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="be069-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="be069-107">Ниже приведены некоторые другие ссылки, которые могут помочь:</span><span class="sxs-lookup"><span data-stu-id="be069-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="be069-108">Как Office 365 использует платформу политики отправителя (SPF) для предотвращения спуфинг</span><span class="sxs-lookup"><span data-stu-id="be069-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="be069-109">Настройка SPF в Office 365 для предотвращения спуфинга</span><span class="sxs-lookup"><span data-stu-id="be069-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

