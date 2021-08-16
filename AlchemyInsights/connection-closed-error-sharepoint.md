---
title: Ошибка "Базовое соединение закрыто" в SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044425"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Ошибка "Базовое соединение закрыто" в SharePoint

Если у вас возникает ошибка "Базовое соединение закрыто" в SharePoint, она может быть связана с прекращением поддержки протокола TLS 1.0/1.1. Дополнительные сведения см. в следующих статьях:

- [Подготовка к TLS 1.2 в Office 365 и Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Возникновение ошибок проверки подлинности, если у клиента нет поддержки TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Если пользователи используют Windows 7, убедитесь, что они проверяют [комплекты шифров TLS в Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).