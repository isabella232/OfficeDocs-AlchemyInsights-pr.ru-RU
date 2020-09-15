---
title: 1554 Winsock Error 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698875"
---
# <a name="winsock-error-10061"></a>Ошибка Winsock 10061

Этот код ошибки означает, что корпорации Майкрософт не удалось установить TCP-сокет (подключение) с конечным узлом. Наиболее вероятная причина этой ошибки — проблема с настройкой брандмауэра. Чтобы устранить эту проблему, проверьте указанные ниже параметры.

- Проверьте конфигурацию брандмауэра, указав сведения в [диапазонах адресов и IP-адресов Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) .

- Если сообщение об ошибке относится только к Exchange Online Protection (EOP), вы уже получали уведомление об изменении [IP-адресов Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Убедитесь, что ваш поставщик услуг Интернета (ISP) не блокирует порт.

- Проверьте параметры промежуточного узла и целевого сервера в соединителях.

Обратите внимание, что Microsoft 365 не блокирует *Входящие* подключения таким образом.
