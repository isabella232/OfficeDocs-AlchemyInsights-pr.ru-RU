---
title: Добавление домена sub
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475986"
---
# <a name="adding-a-sub-domain"></a>Добавление домена sub

В один и тот же или другой клиент могут быть добавлены домены sub, чем родительский. В любом случае необходимо управлять собственными настройками DNS на веб-сайте регистратора. Если вы разрешите Корпорации Майкрософт управлять настройками DNS с помощью записей NS или приобрели домен у Microsoft, вы не можете добавить поддомены, не изменяя это в первую очередь.

Сначала добавьте родительский домен, а затем добавьте под домен. Если поддомен находится в одном и том же клиенте, дополнительная проверка не требуется. При добавлении домена в отдельный клиент запись TXT DNS требуется для проверки прав собственности перед добавлением домена и дополнительных записей DNS для выбранных служб.

- Чтобы добавить домен или поддомена, следуйте мастеру [Добавить](https://admin.microsoft.com/Adminportal#/Domains/Wizard)домен или добавьте домен или subdomain вручную, переехав в **домен Setting**  >  **Domains**  >  **Add**.

При необходимости:

- Чтобы изменить, кто управляет настройками DNS для существующего домена, перейдите в **Параметры**  >  [**Домены,**](https://admin.microsoft.com/Adminportal/Home#/Domains)выберите контрольный ящик рядом с доменом, а затем выберите **Управление DNS**. В мастере выберите **Добавить собственные записи DNS** и завершить мастер.
- Чтобы добавить под домены в приобретенный microsoft домен, сначала передайте домен другому регистратору, а затем внести изменения, чтобы управлять собственными записями DNS. Инструкции см. в [примере Перенос домена из Microsoft в другой хост.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Если вы получаете ошибку, которую ваш домен уже используется другими членами или людьми в вашей организации, прежде чем использовать домен, необходимо сначала учесть эту неугодную учетную запись. Инструкции см. в [статью Take over an unmanaged directory as administrator in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
