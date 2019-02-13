---
title: Ошибка Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903122"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="896ee-102">Ошибка Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="896ee-102">Winsock error 10061</span></span>

<span data-ttu-id="896ee-p101">Этот код ошибки означает, что Office 365 не удалось установить разъем TCP (подключение) с конечного узла. Скорее всего, причиной этой ошибки является проблема связана с вашей конфигурации брандмауэра. Чтобы устранить проблему, проверьте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="896ee-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="896ee-106">Проверка конфигурации брандмауэра со сведениями в [Office 365 URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="896ee-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="896ee-107">Если ошибка относится к Exchange Online Protection (EOP), вы должны ранее уведомлены на внесение изменений в [Exchange Online Protection IP-адреса](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="896ee-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="896ee-108">Убедитесь, что ваше службы поставщика услуг Интернета не блокирует порт.</span><span class="sxs-lookup"><span data-stu-id="896ee-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="896ee-109">Проверьте смарт-параметры узла и целевого сервера в вашей соединители.</span><span class="sxs-lookup"><span data-stu-id="896ee-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="896ee-110">Обратите внимание на то, что Office 365 не блокировать *Входящие* подключения таким образом.</span><span class="sxs-lookup"><span data-stu-id="896ee-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

