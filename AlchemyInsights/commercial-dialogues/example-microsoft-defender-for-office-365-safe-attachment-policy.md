---
title: Пример политики безопасного вложения Microsoft Defender для Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737573"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Пример политики безопасного вложения Microsoft Defender для Office 365

Эти параметры позволяют политике *"Нет* задержки", которая доставляет сообщения сразу, а затем повторно прикрепит вложения после проверки:

- **Имя:** Нет задержек
- **Описание.** Сразу доставляет сообщения и повторно прикрепит вложения после сканирования.
- **Ответ.** Выберите **параметр Динамическая доставка.** Дополнительные сведения см. в [приложении Dynamic Delivery in Safe Attachments policies.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Раздел** Перенаправления вложений. Выберите параметр Включить перенаправление **и** введите адрес электронной почты глобального администратора, администратора безопасности или аналитика безопасности Microsoft 365, который будет исследовать вредоносные вложения.
- **Применяется к разделу:** **Выберите домен получателя,** а затем выберите домен. Выберите **добавить,** а затем выберите **ОК**. По завершению выберите **Сохранить**.

Дополнительные новости см. в [веб-сайте Безопасные вложения в Microsoft Defender для Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
