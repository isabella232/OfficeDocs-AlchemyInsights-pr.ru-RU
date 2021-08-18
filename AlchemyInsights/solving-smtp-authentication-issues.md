---
title: Включение проверки подлинности SMTP и устранение неполадок
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321766"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Включение проверки подлинности SMTP и устранение неполадок

Если вы хотите включить проверку подлинности SMTP для почтового ящика или у вас возникает ошибка "Клиент не прошел проверку подлинности", "Неудачная проверка подлинности" или "SmtpClientAuthentication" с кодом 5.7.57, 5.7.3 или 5.7.139 при попытке ретрансляции электронной почты путем проверки подлинности устройства или приложения в Microsoft 365, выполните три действия для устранения проблемы:

1. Отключите [параметры безопасности по умолчанию Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) путем переключения настройки **Включение параметров безопасности по умолчанию** в положение **Нет**.

    a. Войдите на портал Azure от имени администратора безопасности, администратора условного доступа или глобального администратора.<BR/>
    б. Перейдите в раздел Azure Active Directory > **Свойства**.<BR/>
    в. Выберите **Управление параметрами безопасности по умолчанию**.<BR/>
    г. Присвойте настройке **Включение параметров безопасности по умолчанию** значение **Нет**.<BR/>
    д. Нажмите **Сохранить**.

2. [Включите отправку SMTP клиента](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) в лицензированном почтовом ящике.

    а. В Центре администрирования Microsoft 365 перейдите в раздел **Активные пользователи** и выберите пользователя.<BR/>
    б. Перейдите на вкладку "Почта" и в разделе **Почтовые приложения** выберите **Управление приложениями электронной почты**.<BR/>
    г. Установите флажок **SMTP с проверкой подлинности** (параметр включен).<BR/>
    д. Нажмите **Сохранить изменения**.<BR/>

3. [Отключите многофакторную проверку подлинности (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) в лицензированном почтовом ящике.

    а. Перейдите в Центр администрирования Microsoft 365 и в меню навигации слева выберите **Пользователи** > **Активные пользователи**.<BR/>
    б. Выберите **Многофакторная проверка подлинности**.<BR/>
    в. Выберите пользователя и отключите **многофакторную проверку подлинности**.<BR/>
