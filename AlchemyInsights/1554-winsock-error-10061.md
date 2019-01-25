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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486549"
---
# <a name="winsock-error-10061"></a>Ошибка Winsock 10061

Этот код ошибки означает, что Office 365 не удалось установить разъем TCP (подключение) с конечного узла. Скорее всего, причиной этой ошибки является проблема связана с вашей конфигурации брандмауэра. Чтобы устранить проблему, проверьте следующие параметры:
  
- Проверка конфигурации брандмауэра со сведениями в [Office 365 URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Если ошибка относится к Exchange Online Protection (EOP), вы должны ранее уведомлены на внесение изменений в [Exchange Online Protection IP-адреса](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Убедитесь, что ваше службы поставщика услуг Интернета не блокирует порт.
    
- Проверьте смарт-параметры узла и целевого сервера в вашей соединители.
    
Обратите внимание на то, что Office 365 не блокировать *Входящие* подключения таким образом. 
  

