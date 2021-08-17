---
title: Симулятор атаки 2681 в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895804"
---
# <a name="attack-simulator-in-microsoft-365"></a>Симулятор атаки в Microsoft 365

- Отсутствует симулятор атак? Симулятор атак требует **microsoft Defender для Office 365 плана 2** или Office 365 корпоративный **E5.** Симулятор атак **не входит** в Microsoft Defender для Office 365 плана 1, Office 365 корпоративный E3 или Приложения Microsoft 365 для бизнеса подписки.

- Учетная запись, используемая для запуска имитации атак, требует разрешений глобального администратора или администратора безопасности и многофакторной проверки подлинности (MFA). Дополнительные сведения о требованиях к симулятору атак см. [в этом разделе.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Важные моменты, которые необходимо знать об имитации атак **brute Force Password:**

  - Если в целевой учетной записи включена MFA и пароль был угашен правильно, учетная запись не будет скомпрометирована (второй фактор проверки подлинности будет неполным).

  - Размер файла пароля не может быть больше 10 МБ. Используйте один пароль в строке и включайте пустую строку (возвращение вагона) после последнего пароля в списке.

- Важные моменты, которые необходимо знать о **симуляции приложении к** фишингу копий:

  - По дизайну вы не можете предоставить настраиваемую ценность для **URL-адреса сервера фишинговых входов.**

  - Если получатель использует надстройку [Enable the Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) для сообщения о фишинге, вы можете не получать оповещений о сообщении (так как это имитация атаки).

- Отчеты. После завершения смоделированной атаки можно нажать **кнопку Сведения** о атаке, чтобы увидеть отчет.

- Подробные инструкции и новые функции в симуляторе атак см. в [Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
