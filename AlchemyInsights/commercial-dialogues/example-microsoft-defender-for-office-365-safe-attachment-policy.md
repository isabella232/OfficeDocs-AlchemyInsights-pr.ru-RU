---
title: Пример microsoft Defender для политики Office 365 Сейф вложения
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988308"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Пример microsoft Defender для политики Office 365 Сейф вложения

Эти параметры позволяют политике *"Нет* задержки", которая доставляет сообщения сразу, а затем повторно прикрепит вложения после проверки:

- **Имя:** Нет задержек
- **Описание.** Сразу доставляет сообщения и повторно прикрепит вложения после сканирования.
- **Ответ.** Выберите **параметр Динамическая доставка.** Дополнительные сведения см. в [приложении Dynamic Delivery в Сейф вложениях.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Раздел** Перенаправления вложений. Выберите параметр Включить перенаправление, а затем введите адрес электронной почты глобального администратора Microsoft 365 администратора безопасности или аналитика безопасности, которые будут исследовать вредоносные вложения.
- **Применяется к разделу:** **Выберите домен получателя,** а затем выберите домен. Выберите **добавить,** а затем выберите **ОК**. По завершению выберите **Сохранить**.

Дополнительные новости см. [в Сейф Вложения в Microsoft Defender для Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
