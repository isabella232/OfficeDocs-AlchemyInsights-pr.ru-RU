---
title: Имитатор атак 2681 в Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759232"
---
# <a name="attack-simulator-in-microsoft-365"></a>Симулятор атак в Microsoft 365

- Вы не используете симулятор атак? Для работы в симуляторе атак требуется **office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** или **Office 365 Enterprise**/с. Симулятор атак **не** включен в Office 365 Advanced Threat Protection Plan 1 (ATP, план 1), Office 365 корпоративный E3 или любые приложения Microsoft 365 для бизнес-подписок.

- Для учетной записи, используемой для запуска имитации атак, требуются разрешения администратора глобального администратора или безопасности, а также многофакторную проверку подлинности (MFA). Дополнительные сведения о требованиях к эмулятору атак приведены в [этой статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Важные сведения об управлении атаками **пароля методом грубой силы** :

  - Если для целевой учетной записи включен протокол MFA и правильно выбран пароль, то учетная запись не будет отображаться как скомпрометированная (второй фактор проверки подлинности будет неполным).

  - Размер файла паролей не может превышать 10 МБ. Используйте один пароль для каждой строки и включите пустую строку (возврат каретки) после последнего пароля в списке.

- Важные сведения о имитации имитации **спеар фишинг** -подключения:

  - По дизайну невозможно предоставить настраиваемое значение для **URL-адреса сервера входа в систему фишинга**.

  - Если получатель использует [надстройку "включение сообщения отчета](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " для сообщения о качестве фишинга, вы можете не получать оповещения для этого сообщения (так как это имитация атаки).

- Отчеты: после завершения имитации атаки вы можете просмотреть отчет, щелкнув **сведения об атаках** .

- Подробная информация о новых возможностях и новых возможностях в симуляторе атак приведена [в статье симулятор атак в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
