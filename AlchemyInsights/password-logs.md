---
title: Журналы паролей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960956"
---
# <a name="password-logs"></a>Журналы паролей

**У меня возникли проблемы с доступом к журналам аудита сброса пароля**

Чтобы устранить проблемы с доступом к журналам аудита сброса пароля, выполните следующее действие:

Убедитесь, что у вас есть права на просмотр журналов аудита. 

Такие права имеют только следующие роли:
 - Глобальный администратор
 - Администратор безопасности
 - Читатель безопасности

**Мне нужно просмотреть все события аудита сброса пароля с момента начального развертывания**

В отчетах за последние 30 дней хранится до 120 000 событий регистрации или сброса пароля. Это максимально допустимое число для пользовательского интерфейса при загрузке CSV-файла. 1 млн событий доступен через PowerShell.
Дополнительные сведения см. по указанным ниже ссылкам.

- [События самостоятельного сброса пароля из API отчетов и событий Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Быстрое скачивание событий регистрации для сброса пароля с помощью PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Мне нужны дополнительные сведения о возможностях создания отчетов о сбросе пароля**

Узнайте, кто регистрируется для сброса или сбрасывает пароль, с помощью журналов аудита сброса пароля Azure AD на портале Azure в разделе **Пользователи и группы**.
Дополнительные сведения см. по указанным ниже ссылкам.

- [Обзор отчетов о сбросе пароля](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Как просматривать отчеты о сбросе пароля на портале Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [События самостоятельного сброса пароля из API отчетов и событий Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Быстрое скачивание событий регистрации для сброса пароля с помощью PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


