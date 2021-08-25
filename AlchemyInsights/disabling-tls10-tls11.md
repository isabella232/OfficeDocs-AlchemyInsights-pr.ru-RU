---
title: Отключение TLS1.0 и TLS 1.1 для отправки клиента SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58380679"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Отключение TLS1.0 и TLS 1.1 для отправки клиента SMTP AUTH

Недавно мы начали отключать TLS1.0 и TLS 1.1 для отправки клиента SMTP AUTH. 

Если вы настроили устройство, приложение или сервер, которые отправляют электронную почту в Microsoft 365 с помощью метода отправки клиента SMTP AUTH, убедитесь, что ваше устройство, приложение или сервер поддерживают TLS 1.2 для SMTP. 