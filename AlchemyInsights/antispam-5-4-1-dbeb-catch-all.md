---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821460"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Устранение проблем с доставкой для кода ошибки 550 5.4.1 Отказ в ретрансляторе доступа

Эта проблема возникает при [проверке](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) допустимого адреса электронной почты для предотвращения отскоков при входе в сеть Майкрософт. Попробуйте следующее:

1. Определите, является ли проблема конкретной для всего домена или одного адреса электронной почты:
    - Весь домен. Иногда необходимо синхронизировать домен; попробуйте [установить домен на Внутренний, а затем вернуться к авторитетному](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Единый адрес электронной почты. Иногда требуется синхронизировать адрес; изменение прокси-адреса smtp и его обратное изменение может помочь.
2. Определите, является ли проблема конкретной для группы или общедоступных папок. Для некоторых типов объектов может потребоваться вручную создавать объекты в Azure Active Directory.

Если вам нужна дополнительная помощь, откройте билет поддержки и укажите область проблемы (в том числе тип объекта, в который вы отправляете), чтобы мы могли помочь вам лучше.