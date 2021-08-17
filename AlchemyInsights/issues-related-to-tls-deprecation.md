---
title: Невозможность отправки и получения электронной почты в/Office 365 из-за отключения TLS 1.0 и TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054919"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Невозможность отправки и получения электронной почты в/Office 365 из-за отключения TLS 1.0 и TLS 1.1

Как подтвердило сообщение центра сообщений post MC229914, обесценение TLS 1.0 и TLS 1.1 началось для Exchange Online конечных точек потока почты. Скоро Office 365 больше не будут принимать подключения к электронной почте TLS 1.0 и TLS 1.1 из внешних источников. Кроме того, Exchange Online никогда не будет использовать TLS 1.0 или 1.1 для отправки исходящие сообщения электронной почты. Если у вас возникнут проблемы из-за отключения TLS 1.0 или 1.1, может возникнуть одна из следующих ошибок:

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Ошибка в просмотра очереди локального сервера, отправляемого по электронной почте сотруднику 365- '421 4.4.2 Подключение, отброшенное из-за SocketError'
- Ошибка в журнале Протокола протокола отправки соединителя на сервере, отправляемом электронной почте Office 365- TLS, не удалось с ошибкой SocketError [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)
- Ошибка в журнале протокола отправки или получения соединителя - '451 5.7.3 Сначала необходимо издать команду STARTTLS'

Если вы испытываете все вышеперечисленные ошибки, убедитесь, что сервер, который отправляет или получает электронную почту, включен tLS 1.2, проверяя следующие клавиши реестра.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Если вы внося изменения в вышеуказанные клавиши реестра, чтобы включить TLS 1.2, перезапустите сервер, чтобы изменения вступили в силу. Кроме того, убедитесь, что у вас Windows и Exchange обновления.

Дополнительные сведения см. в указанных ниже статьях.

- [Exchange Server Руководство TLS, часть 1. Получение готовности к TLS 1.2 — microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Руководство TLS Часть 2. Включение TLS 1.2 и определение клиентов, не использующих его, — Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Понимание сценариев электронной почты, если версии TLS не могут быть согласованы с Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
