---
title: Настройка DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808720"
---
# <a name="setup-dkim"></a>Настройка DKIM

В [этой статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)приведены полные инструкции по настройке DKIM для пользовательских доменов в Microsoft 365.

1. Для **каждого** настраиваемого домена необходимо создать **две** записи CNAME DKIM в службе хостинга DNS вашего домена (обычно это регистратор доменных имен). Например, contoso.com и fourthcoffee.com должны иметь четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.

   Записи CNAME DKIM для **каждого** пользовательского домена используют следующие форматы:

   - **Имя узла**: `selector1._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Имя узла**: `selector2._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> — Это текст, расположенный слева `.mail.protection.outlook.com` в настраиваемой записи MX для пользовательского домена (например, `contoso-com` для домена contoso.com). \<InitialDomain\> — Это домен, который вы использовали при регистрации в Microsoft 365 (например, contoso.onmicrosoft.com).

2. Создав записи CNAME для пользовательских доменов, выполните следующие действия:

   а. [Войдите в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с помощью рабочей или учебной учетной записи.

   б. В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.

   в. В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.

   г. Перейдите в раздел **Защита**  >  **DKIM**.

   д. Выберите домен, а затем выберите **включить** для **подписи сообщений для этого домена с DKIM подписями**. Повторите этот шаг для каждого личного домена.
