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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324003"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Устранение распространенных проблем с форматированием записей DKIM

Большинство проблем с настройками DKIM связаны с неправильными записями DNS.

Чтобы устранить проблемы с настройками DKIM, убедитесь, что запись DKIM CNAME **(а** не запись TXT) отформатирована правильно. Дополнительные сведения см. в дополнительных сведениях о том, что необходимо сделать, чтобы вручную настроить [DKIM в Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Если вам нужна помощь с записями DNS в целом, см. в справке [Create DNS records at any DNS hosting provider for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Примечание.** После создания или обновления записей DKIM DNS в службе размещения DNS для домена необходимо дождаться распространения записей DNS.
