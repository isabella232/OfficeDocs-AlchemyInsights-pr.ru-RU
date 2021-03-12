---
title: Невозможность отправки и получения электронной почты в/из Office 365 из-за отключения TLS 1.0 и TLS 1.1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726937"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="01bba-102">Невозможность отправки и получения электронной почты в/из Office 365 из-за отключения TLS 1.0 и TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="01bba-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="01bba-103">Как подтвердила почта центра сообщений MC229914, обесценение TLS 1.0 и TLS 1.1 стало применяться для конечных точек потока почты Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="01bba-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="01bba-104">Вскоре Office 365 больше не будет принимать подключения к электронной почте TLS 1.0 и TLS 1.1 из внешних источников.</span><span class="sxs-lookup"><span data-stu-id="01bba-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="01bba-105">Кроме того, Exchange Online никогда не будет использовать TLS 1.0 или 1.1 для отправки исходящие сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01bba-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="01bba-106">Если у вас возникнут проблемы из-за отключения TLS 1.0 или 1.1, может возникнуть одна из следующих ошибок:</span><span class="sxs-lookup"><span data-stu-id="01bba-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="01bba-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="01bba-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="01bba-108">Ошибка в просмотра очереди локального сервера, отправляемого по электронной почте сотруднику 365- '421 4.4.2 Подключение, отброшенное из-за SocketError'</span><span class="sxs-lookup"><span data-stu-id="01bba-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="01bba-109">Ошибка в журнале протокола отправки [соединителя](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) на сервере отправки электронной почты в Office 365- TLS не удалось с ошибкой SocketError</span><span class="sxs-lookup"><span data-stu-id="01bba-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="01bba-110">Ошибка в журнале протокола отправки или получения соединителя - '451 5.7.3 Сначала необходимо издать команду STARTTLS'</span><span class="sxs-lookup"><span data-stu-id="01bba-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="01bba-111">Если вы испытываете все вышеперечисленные ошибки, убедитесь, что сервер, который отправляет или получает электронную почту, включен tLS 1.2, проверяя следующие клавиши реестра.</span><span class="sxs-lookup"><span data-stu-id="01bba-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="01bba-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:0000000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="01bba-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="01bba-113">Если вы внося изменения в вышеуказанные клавиши реестра, чтобы включить TLS 1.2, перезапустите сервер, чтобы изменения вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="01bba-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="01bba-114">Кроме того, убедитесь, что у вас установлены последние обновления Windows и Exchange.</span><span class="sxs-lookup"><span data-stu-id="01bba-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="01bba-115">Дополнительные сведения см. в статьях:</span><span class="sxs-lookup"><span data-stu-id="01bba-115">For more information, see:</span></span>

- [<span data-ttu-id="01bba-116">Exchange Server TLS, часть 1. Готовимся к TLS 1.2 — microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="01bba-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="01bba-117">Exchange Server TLS Руководство Часть 2: Включение TLS 1.2 и определение клиентов, не использующих его , - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="01bba-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="01bba-118">Понимание сценариев электронной почты, если версии TLS не могут быть согласованы с Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="01bba-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
