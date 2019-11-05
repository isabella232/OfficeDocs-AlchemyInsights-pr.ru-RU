---
title: Защиты от спама 5.4.1 DBEB Catch — All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964287"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Устранение проблем с доставкой для ошибки с кодом 550 5.4.1 отказ в доступе к ретрансляции

Эта проблема возникает в тех случаях, когда [проверяется допустимость адреса электронной почты для предотвращения баунцебаккс](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при входе в сеть Office 365. Попробуйте выполнить следующие действия:

1. Определите, относится ли проблема к целому домену или к одному адресу электронной почты:
    - Весь домен: иногда требуется синхронизация домена; Попробуйте [присвоить домену значение Internal, а затем обратно в значение заслуживающий доверия](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Один адрес электронной почты: иногда необходимо синхронизировать адрес; изменение SMTP-адреса прокси-сервера и его изменение обратно может помочь.
2. Определите, характерна ли проблема для группы или общедоступной папки. Для некоторых типов объектов может потребоваться вручную создать объекты в Azure Active Directory.

Если вам нужна дополнительная помощь, откройте билет поддержки и укажите область ее действия (инклудиднг тип объекта, на который вы отправляетесь), чтобы мы могли помочь вам лучше.