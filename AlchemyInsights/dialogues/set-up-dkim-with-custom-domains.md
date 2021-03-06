---
title: Настройка DKIM с помощью настраиваемого домена
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500958"
---
# <a name="set-up-dkim-with-custom-domains"></a>Настройка DKIM с помощью настраиваемого домена

Необходимо опубликовать две записи CNAME для каждого пользовательского домена в DNS. Для этого используйте следующий формат:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** — это текст слева **от .mail.protection.outlook.com** в настраиваемой записи MX для настраиваемого домена (например, contoso-com **для домена contoso.com).** **InitialDomain** — это домен, используемый при регистрации на Office 365 (например, **contoso.onmicrosoft.com).**

Дополнительные сведения о записях DNS см. в руб. Создание записей DNS в любом [поставщике DNS-хостинга для Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)