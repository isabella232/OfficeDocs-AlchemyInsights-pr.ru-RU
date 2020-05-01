---
title: Настройка DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645685"
---
# <a name="setup-dkim"></a>Настройка DKIM

В [этой статье](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)приведены полные инструкции по настройке DKIM для пользовательских доменов в Microsoft 365.

1. Для **каждого** настраиваемого домена необходимо создать **две** записи CNAME DKIM в службе хостинга DNS вашего домена (обычно это регистратор доменных имен). Например, contoso.com и fourthcoffee.com должны иметь четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.

   Записи CNAME DKIM для **каждого** пользовательского домена используют следующие форматы:

   - **Имя узла**:`selector1._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Имя узла**:`selector2._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> — текст слева от `.mail.protection.outlook.com` настраиваемой записи MX для пользовательского домена (например, `contoso-com` для домена contoso.com). \<Инитиалдомаин\> — это домен, который вы использовали при регистрации в Microsoft 365 (например, contoso.onmicrosoft.com).

2. Создав записи CNAME для пользовательских доменов, выполните следующие действия:

   а. [Войдите в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с помощью рабочей или учебной учетной записи.

   б) В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.

   в. В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.

   г. Перейдите в раздел **Защита** > **DKIM**.

   д. Выберите домен, а затем выберите **включить** для **подписи сообщений для этого домена с DKIM подписями**. Повторите этот шаг для каждого личного домена.
