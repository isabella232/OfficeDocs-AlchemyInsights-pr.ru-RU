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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326810"
---
# <a name="fix-tenant-policy-action-override"></a>Исправлена политика клиента (переопределения действий)

Одна из ваших политик по борьбе со спамом повлияла на это сообщение. Чтобы просмотреть политики, сделайте следующие действия:

1. На портале Microsoft 365 Defender в разделе Политики совместной & электронной почты & правила политики угрозы в разделе <https://security.microsoft.com/>  \>  \>  \>  **Политики.**

   Чтобы сразу перейти к странице **Политики защиты от нежелательной почты**, используйте ссылку <https://security.microsoft.com/antispam>.

2. На странице Политики по борьбе со спамом выберите политику, нажав на имя политики **(Type** is Custom **anti-spam** **policy** or **Name** is **Anti-Spam inbound policy (Default).**
3. В подробной вылете, которая появится, выберите **Изменить действия в** разделе **Действия.**
4. В разделе Действия **сообщения** просмотрите вердикты для спама, высокой уверенности в спаме, фишинге и фишинге с высокой уверенностью, чтобы узнать, выбрано ли любое из следующих значений:    
   - **Добавить X-заголовок**
   - **Добавить в начало темы текст**
   - **Перенаправление сообщения на адрес электронной почты**
   - **Удалить сообщение**
   - **Нет действий**

   Не исключено,  что стандартные параметры, применяемые Exchange Online Protection пользователей, повлияли на сообщение.

Дополнительные сведения см. в статье [Настройка политик защиты от спама в EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
