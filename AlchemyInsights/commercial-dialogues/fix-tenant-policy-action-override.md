---
title: Исправлена политика клиента (переопределения действий)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034947"
---
# <a name="fix-tenant-policy-action-override"></a>Исправлена политика клиента (переопределения действий)

Политика борьбы со спамом в клиенте повлияла на это сообщение. Чтобы просмотреть политику, сделайте следующее:

1. Перейдите в [центр Office 365 безопасности &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)а затем перейдите в центр по борьбе со спамом политики управления   >    >  [угрозами.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Проверьте, **указывает** ли источник политики следующее:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Если это так, на **вкладке Custom** проверьте параметры политики, которая повлияла на сообщение. Не исключено,  что стандартные параметры, применяемые Exchange Online Protection пользователей, повлияли на сообщение.

Дополнительные сведения о настройке политик фильтрации нежелательной почты см. в дополнительных сведениях о настройке политик фильтра [нежелательной почты.](https://go.microsoft.com/fwlink/?linkid=2101431)
