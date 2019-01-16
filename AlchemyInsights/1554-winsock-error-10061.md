---
title: Ошибка Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308205"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2680d-102">Ошибка Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="2680d-102">Winsock error 10061</span></span>

<span data-ttu-id="2680d-p101">Этот код ошибки означает, что Office 365 не удалось установить разъем TCP (подключение) с конечного узла. Скорее всего, причиной этой ошибки является проблема связана с вашей конфигурации брандмауэра. Чтобы устранить проблему, проверьте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="2680d-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="2680d-106">Проверка конфигурации брандмауэра со сведениями в [Office 365 URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2680d-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="2680d-107">Если ошибка относится к Exchange Online Protection (EOP), вы должны ранее уведомлены на внесение изменений в [Exchange Online Protection IP-адреса](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2680d-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="2680d-108">Убедитесь, что ваше службы поставщика услуг Интернета не блокирует порт.</span><span class="sxs-lookup"><span data-stu-id="2680d-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="2680d-109">Проверьте смарт-параметры узла и целевого сервера в вашей соединители.</span><span class="sxs-lookup"><span data-stu-id="2680d-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="2680d-110">Обратите внимание на то, что Office 365 не блокировать *Входящие* подключения таким образом.</span><span class="sxs-lookup"><span data-stu-id="2680d-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

