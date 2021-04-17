---
title: Решение проблем аутентификации SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826428"
---
# <a name="solving-smtp-authentication-issues"></a>Решение проблем аутентификации SMTP

Если вы получаете ошибки 5.7.57 или 5.7.3 при попытке отправки электронной почты SMTP и аутентификации с помощью клиента или приложения, необходимо проверить несколько вещей:

- Аутентифицированная отправка SMTP может быть отключена в вашем клиенте или в почтовом ящике, который вы пытаетесь использовать (проверьте обе настройки). Подробнее читайте в разделе [Включение или отключение отправки SMTP аутентифицированного клиента](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Проверьте, включены ли [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для вашего клиента; если включено, SMTP-аутентификация с использованием базовой аутентификации (также известной как устаревшая; при этом будут использоваться имя пользователя и пароль) не будет выполнена.
