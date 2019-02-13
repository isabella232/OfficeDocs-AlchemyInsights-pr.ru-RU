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
# <a name="winsock-error-10061"></a>Ошибка Winsock 10061

Этот код ошибки означает, что Office 365 не удалось установить разъем TCP (подключение) с конечного узла. Скорее всего, причиной этой ошибки является проблема связана с вашей конфигурации брандмауэра. Чтобы устранить проблему, проверьте следующие параметры:
  
- Проверка конфигурации брандмауэра со сведениями в [Office 365 URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Если ошибка относится к Exchange Online Protection (EOP), вы должны ранее уведомлены на внесение изменений в [Exchange Online Protection IP-адреса](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Убедитесь, что ваше службы поставщика услуг Интернета не блокирует порт.
    
- Проверьте смарт-параметры узла и целевого сервера в вашей соединители.
    
Обратите внимание на то, что Office 365 не блокировать *Входящие* подключения таким образом. 
  

