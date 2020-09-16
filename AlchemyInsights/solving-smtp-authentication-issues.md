---
title: Решение проблем аутентификации SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738002"
---
# <a name="solving-smtp-authentication-issues"></a>Решение проблем аутентификации SMTP

Если вы получаете ошибки 5.7.57 или 5.7.3 при попытке отправки электронной почты SMTP и аутентификации с помощью клиента или приложения, необходимо проверить несколько вещей:

- Аутентифицированная отправка SMTP может быть отключена в вашем клиенте или в почтовом ящике, который вы пытаетесь использовать (проверьте обе настройки). Подробнее читайте в разделе [Включение или отключение отправки SMTP аутентифицированного клиента](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Проверьте, включены ли [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для вашего клиента; если включено, SMTP-аутентификация с использованием базовой аутентификации (также известной как устаревшая; при этом будут использоваться имя пользователя и пароль) не будет выполнена.
