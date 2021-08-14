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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932290"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Устранение проблем с доставкой для кода ошибки 550 5.4.1 Отказ в ретрансляторе доступа

Эта проблема возникает при [проверке](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) допустимого адреса электронной почты для предотвращения отскоков при входе в сеть Майкрософт. Попробуйте следующее:

1. Определите, является ли проблема конкретной для всего домена или одного адреса электронной почты:
    - Весь домен. Иногда необходимо синхронизировать домен; попробуйте [установить домен на Внутренний, а затем вернуться к авторитетному](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Единый адрес электронной почты. Иногда требуется синхронизировать адрес; изменение прокси-адреса smtp и его обратное изменение может помочь.
2. Определите, является ли проблема конкретной для группы или общедоступных папок. Для некоторых типов объектов может потребоваться вручную создавать объекты в Azure Active Directory.

Если вам нужна дополнительная помощь, откройте билет поддержки и укажите область проблемы (в том числе тип объекта, в который вы отправляете), чтобы мы могли помочь вам лучше.