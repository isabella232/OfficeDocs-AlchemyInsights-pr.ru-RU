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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919040"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Ошибка "401 Не авторизовано" в SharePoint

Если вы получаете сообщение об ошибке "(401) Не авторизовано" в SharePoint, эта ошибка может быть связана с упразднением TLS 1.0/1.1. Дополнительные сведения см. в:

- [Подготовка к TLS 1.2 в Office 365 и Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Возникновение ошибок проверки подлинности, если у клиента нет поддержки TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Если пользователи используют Windows 7, убедитесь, что они проверяют [комплекты шифров TLS в Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).