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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545739"
---
# <a name="attack-simulator-in-microsoft-365"></a>Симулятор атаки в Microsoft 365

- Отсутствует симулятор атак? Симулятор атак требует **microsoft Defender для Office 365 плана 2** или Office 365 корпоративный **E5.** Симулятор атак **не входит** в Microsoft Defender для Office 365 плана 1, Office 365 корпоративный E3 или Приложения Microsoft 365 для бизнеса подписки.

- Учетная запись, используемая для запуска имитации атак, требует разрешений глобального администратора или администратора безопасности и многофакторной проверки подлинности (MFA). Дополнительные сведения о требованиях к симулятору атак см. [в этом разделе.](/microsoft-365/security/office-365-security/attack-simulator)

- Важные моменты, которые необходимо знать об имитации атак **brute Force Password:**

  - Если в целевой учетной записи включена MFA и пароль был угашен правильно, учетная запись не будет скомпрометирована (второй фактор проверки подлинности будет неполным).

  - Размер файла пароля не может быть больше 10 МБ. Используйте один пароль в строке и включайте пустую строку (возвращение вагона) после последнего пароля в списке.

- Важные моменты, которые необходимо знать о **симуляции приложении к** фишингу копий:

  - По дизайну вы не можете предоставить настраиваемую ценность для **URL-адреса сервера фишинговых входов.**

  - Если получатель использует надстройку [Enable the Report Message](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) для сообщения о фишинге, вы можете не получать оповещений о сообщении (так как это имитация атаки).

- Отчеты. После завершения смоделированной атаки можно нажать **кнопку Сведения** о атаке, чтобы увидеть отчет.

- Подробные инструкции и новые функции в симуляторе атак см. в [Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)
