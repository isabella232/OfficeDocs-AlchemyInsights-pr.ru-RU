---
title: 1554 Winsock Error 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530817"
---
# <a name="winsock-error-10061"></a>Ошибка Winsock 10061

Этот код ошибки означает, что Office 365 не удалось установить TCP-сокет (подключение) к конечному узлу. Наиболее вероятная причина этой ошибки — проблема с настройкой брандмауэра. Чтобы устранить эту проблему, проверьте указанные ниже параметры.

- Проверьте конфигурацию брандмауэра, указав сведения в [диапазонах адресов и IP-адресов Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) .

- Если сообщение об ошибке относится только к Exchange Online Protection (EOP), вы уже получали уведомление об изменении [IP-адресов Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Убедитесь, что ваш поставщик услуг Интернета (ISP) не блокирует порт.

- Проверьте параметры промежуточного узла и целевого сервера в соединителях.

Обратите внимание, что Office 365 не блокирует *Входящие* подключения таким образом.
