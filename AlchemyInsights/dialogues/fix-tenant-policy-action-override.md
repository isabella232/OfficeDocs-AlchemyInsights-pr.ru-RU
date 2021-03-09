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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552527"
---
# <a name="fix-tenant-policy-action-override"></a>Исправлена политика клиента (переопределения действий)

Политика борьбы со спамом в клиенте повлияла на это сообщение. Чтобы просмотреть политику, сделайте следующее:

1. Перейдите в Центр обеспечения безопасности [Office 365 &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)а затем перейдите в центр по борьбе со спамом политики управления   >    >  [угрозами.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Проверьте, **указывает** ли источник политики следующее:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Если это так, на **вкладке Custom** проверьте параметры политики, которая повлияла на сообщение. Не исключено, что стандартные **параметры,** применяемые для всех клиентов Exchange Online Protection, повлияли на сообщение.

Дополнительные сведения о настройке политик фильтрации нежелательной почты см. в дополнительных сведениях о настройке политик фильтра [нежелательной почты.](https://go.microsoft.com/fwlink/?linkid=2101431)
