---
title: 'Бизнес-правила Dynamics 365: бизнес-правило не срабатывает для формы'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529032"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Событие OnChange не происходит, если поле изменяется программным способом

Событие *onChange* не происходит, если поле изменяется программным способом с помощью *атрибута.* метод [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Если вы хотите, чтобы обработчики событий для события *onChange* выполнялись после установки значения, необходимо использовать *атрибут формконтекст. Data. Entity.* метод [фиреончанже](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) в коде.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
