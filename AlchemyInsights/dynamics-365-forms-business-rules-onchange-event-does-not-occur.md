---
title: Dynamics 365 Forms Business Rules - Business Rule Not Firing for a Form
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947312"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Событие OnChange не происходит, если поле изменено программным образом

Событие *OnChange* не происходит, если поле изменено программным образом с помощью *атрибута.* [метод setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Если вы хотите, чтобы обработчики событий для *события OnChange* запускались после набора значения, необходимо использовать метод [fireOnchange атрибута fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) в коде *formContext.data.entity.*

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
