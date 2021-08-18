---
title: OneDrive входа AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112925"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive входа AADSTS50011

Если вы получаете ошибку "AADSTS50011: URL-адрес ответа, указанный в запросе, не соответствует ответу" при входе в приложение OneDrive, проверьте следующее:

Ваша OneDrive должна быть равна или больше версии 20.052.XXXX.XXXX. Чтобы проверить свою версию, щелкните значок OneDrive в области уведомлений, выберите справку **& Параметры > Параметры > о**.

Сеть может блокировать трафик для **g.live.com** **и oneclient.sfx.ms.** Если этот трафик заблокирован, OneDrive не удается обновиться. Работайте с сетевым администратором, чтобы обеспечить доступ к этим URL-адресам. [Эти конечные точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) должны быть понятны для клиентов, использующих Microsoft 365 планов.

Если вам нужно вручную получить текущую версию OneDrive, посетите [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
