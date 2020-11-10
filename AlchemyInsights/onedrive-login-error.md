---
title: Ошибка входа в OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947504"
---
# <a name="onedrive-login-error-aadsts50011"></a>Ошибка входа в OneDrive AADSTS50011

При получении сообщения об ошибке "AADSTS50011: URL-адрес ответа, указанный в запросе, не отвечает" при входе в приложение OneDrive, проверьте следующее:

Версия OneDrive должна быть больше или равна версии 20.052. XXXX. Означает. Чтобы проверить версию, щелкните синий значок OneDrive в области уведомлений, выберите **раздел справка & параметры > параметры > о**.

Сеть может блокировать трафик в **g.Live.com** и **oneclient.SFX.MS**. Если этот трафик блокируется, OneDrive не сможет обновить себя. Свяжитесь с администратором сети, чтобы убедиться, что у вас есть доступ к этим URL-адресам. [Эти конечные точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) должны быть достижимыми для клиентов, использующих планы Microsoft 365.

Если вам нужно получить текущую версию OneDrive вручную, посетите страницу [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
