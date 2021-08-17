---
title: Ошибка 1554 Winsock 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083243"
---
# <a name="winsock-error-10061"></a>Ошибка Winsock 10061

Этот код ошибки означает, что Корпорация Майкрософт не смогла установить розетку TCP (подключение) с целевым хостом. Наиболее вероятной причиной этой ошибки является проблема с конфигурацией брандмауэра. Чтобы устранить проблему, проверьте эти параметры:

- Проверка конфигурации брандмауэра с помощью [Microsoft 365 URL-адресов и IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Если ошибка является определенной для Exchange Online Protection (EOP), вы должны были быть предварительно уведомлены об изменении Exchange Online Protection [IP-адресов](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Убедитесь, что поставщик интернет-услуг (ISP) не блокирует порт.

- Проверка параметров интеллектуального хоста и целевого сервера в соединители.

Обратите внимание, Microsoft 365 не *блокирует* входящие подключения таким образом.
