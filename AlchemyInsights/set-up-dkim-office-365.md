---
title: Установка DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108569"
---
# <a name="setup-dkim"></a>Установка DKIM

Полные инструкции по настройке DKIM для настраиваемых доменов в Microsoft 365 [здесь](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Для **каждого** настраиваемого домена необходимо создать две записи **DKIM** CNAME в службе DNS-хостинга домена (как правило, регистратора домена). Например, contoso.com и fourthcoffee.com требуются четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.

   Записи DKIM CNAME для **каждого** настраиваемого домена используют следующие форматы:

   - **Имя хозяина:**`selector1._domainkey.<CustomDomain>`

     **Указывает на адрес или значение:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Имя хозяина:**`selector2._domainkey.<CustomDomain>`

     **Указывает на адрес или значение:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> — это текст слева от настраиваемой записи MX для настраиваемого `.mail.protection.outlook.com` домена (например, для `contoso-com` домена contoso.com). \<InitialDomain\>это домен, используемый при регистрации на Microsoft 365 (например, contoso.onmicrosoft.com).

2. После создания записей CNAME для пользовательских доменов выполните следующие инструкции:

   А. [во входе Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с вашей учетной записью или учебной записью.

   Б. В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.

   c. В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.

   d. Перейдите **к защите**  >  **DKIM**.

   e. Выберите домен, а затем **выберите Включить** для подписи сообщения для этого домена с **помощью подписей DKIM.** Повторите этот шаг для каждого личного домена.
