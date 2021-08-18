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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332320"
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
**Примечание.** **DomainGUID** — это текст слева **от .mail.protection.outlook.com** в настраиваемой записи MX для настраиваемого домена (например, contoso-com для **домена contoso.com).** **InitialDomain** — это домен, используемый при регистрации на Office 365 (например, **contoso.onmicrosoft.com).**

Дополнительные сведения о записях DNS см. в записях создания DNS в любом [поставщике DNS-хостинга для Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)