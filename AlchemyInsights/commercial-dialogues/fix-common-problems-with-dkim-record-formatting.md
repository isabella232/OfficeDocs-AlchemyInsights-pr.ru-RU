---
title: Устранение распространенных проблем с форматированием записей DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930074"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Устранение распространенных проблем с форматированием записей DKIM

Большинство проблем с настройками DKIM связаны с неправильными записями DNS.

Чтобы устранить проблемы с настройками DKIM, убедитесь, что запись DKIM CNAME **(а** не запись TXT) отформатирована правильно. Дополнительные сведения см. в дополнительных сведениях о том, что необходимо сделать, чтобы вручную настроить [DKIM в Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Если вам нужна помощь с записями DNS в целом, см. в справке [Create DNS records at any DNS hosting provider for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> После создания или обновления записей DKIM DNS в службе размещения DNS для домена необходимо дождаться распространения записей DNS.
