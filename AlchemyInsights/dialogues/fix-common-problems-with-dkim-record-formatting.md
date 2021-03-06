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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50501053"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Устранение распространенных проблем с форматированием записей DKIM

Большинство проблем с настройками DKIM связаны с неправильными записями DNS.

Чтобы устранить проблемы с настройками DKIM, убедитесь, что запись DKIM CNAME **(а** не запись TXT) отформатирована правильно. Дополнительные сведения см. в рубрике Что нужно сделать для вручную настроить [DKIM в Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Если вам нужна помощь с записями DNS в целом, см. в справке [Create DNS records at any DNS hosting provider for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> После создания или обновления записей DKIM DNS в службе размещения DNS для домена необходимо дождаться распространения записей DNS.
