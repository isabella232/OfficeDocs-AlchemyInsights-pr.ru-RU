---
title: Устранение распространенных проблем с Microsoft Defender для Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330073"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Устранение распространенных проблем с Microsoft Defender для Office 365

Вот несколько решений распространенных проблем с Microsoft Defender для Office 365:

- **Задержка сообщения:**

  Задержки с доставкой электронной почты могут быть Сейф проверки вложений сообщений. Дополнительные сведения см. [в Сейф параметры политики вложений.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Сообщение о ложных положительных или отрицательных результатах:**

  Для получения дополнительной информации см. [Отчет о сообщениях и файлах в Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Включить защиту Сейф ссылки:**

  1. На портале Microsoft 365 Defender перейдите на электронную почту & политики совместной & правила угрозы Сейф <https://security.microsoft.com/>  \>  \>  \> **ссылки** в разделе **Политики.**

     Чтобы перейти непосредственно **на страницу Сейф ссылки,** используйте <https://security.microsoft.com/safelinksv2> .

  2. На странице **Сейф ссылки** выберите политику, нажав на имя политики.
  3. В вылете сведений, которые появляются, сделайте любой из следующих действий:
     - Чтобы добавить новую политику, выберите **+ Создать**. Мастер запустится, чтобы помочь вам определить параметры политики.
     - Чтобы изменить существующую политику, выберите политику, нажав на имя политики. В подробной вылете, которая появится, выберите **Изменить** в разделе **Параметры защиты.**
  4. На странице **Параметры защиты** настройте следующие параметры:
     - **Включив выберите действие для неизвестных потенциально вредоносных URL-адресов в сообщениях.**
     - Выберите **Применение безопасных ссылок на сообщения, отправленные в организации.**

  Дополнительные сведения см. в Сейф ссылки в [Microsoft Defender для Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
