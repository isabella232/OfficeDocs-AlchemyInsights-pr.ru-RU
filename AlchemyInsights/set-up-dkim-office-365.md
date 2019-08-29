---
title: Настройка DKIM в Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666277"
---
# <a name="setup-dkim-in-office-365"></a>Настройка DKIM в Office 365

В [этой статье](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)приведены полные инструкции по настройке DKIM для пользовательских доменов в Office 365.

1. Для **каждого** настраиваемого домена необходимо создать **две** записи CNAME DKIM в службе хостинга DNS вашего домена (обычно это регистратор доменных имен). Например, contoso.com и fourthcoffee.com должны иметь четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.

   Записи CNAME DKIM для **каждого** пользовательского домена используют следующие форматы:

   - **Имя узла**:`selector1._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Имя узла**:`selector2._domainkey.<CustomDomain>`

     **Указывает на адрес или значение**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> — текст слева от `.mail.protection.outlook.com` настраиваемой записи MX для пользовательского домена (например, `contoso-com` для домена contoso.com). \<Инитиалдомаин\> — это домен, который вы использовали при регистрации в Office 365 (например, contoso.onmicrosoft.com).

2. Создав записи CNAME для пользовательских доменов, выполните следующие действия:

   а. [Войдите в Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с помощью рабочая или учебная учетная запись.

   б) В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.

   В. В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.

   Г. Перейдите в раздел **Защита** > **DKIM**.

   Д. Выберите домен, а затем выберите **включить** для **подписи сообщений для этого домена с DKIM подписями**. Повторите этот шаг для каждого личного домена.
