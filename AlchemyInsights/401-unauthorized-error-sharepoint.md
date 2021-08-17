---
title: Ошибка "401 Не авторизовано" в SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314361"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Ошибка "401 Не авторизовано" в SharePoint

Если вы получаете сообщение об ошибке "(401) Не авторизовано" в SharePoint, эта ошибка может быть связана с упразднением TLS 1.0/1.1. Дополнительные сведения см. в:

- [Подготовка к TLS 1.2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Возникновение ошибок проверки подлинности, если у клиента нет поддержки TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Если пользователи используют Windows 7, убедитесь, что они проверяют [комплекты шифров TLS в Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).