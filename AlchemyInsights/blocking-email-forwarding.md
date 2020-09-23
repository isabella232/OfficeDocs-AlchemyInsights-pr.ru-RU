---
title: 726 блокировка переадресации электронной почты
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219868"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="68558-102">Блокировка или разблокировка переадресации электронной почты</span><span class="sxs-lookup"><span data-stu-id="68558-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="68558-103">Чтобы включить или отключить переадресацию электронной почты для определенного почтового ящика, ознакомьтесь со статьей [Настройка переадресации электронной почты](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="68558-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="68558-104">На уровне клиента управление внешней пересылкой выполняется с помощью политики исходящих сообщений о нежелательной почте.</span><span class="sxs-lookup"><span data-stu-id="68558-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="68558-105">Если этот параметр имеет значение "отключено" или "автоматически", он может блокировать переадресацию электронной почты с сообщением "550 5.7.520 Access Denied, ваша организация не разрешает внешнюю переадресацию".</span><span class="sxs-lookup"><span data-stu-id="68558-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="68558-106">Если пересылка заблокирована, то это ошибка, которую увидят пользователи.</span><span class="sxs-lookup"><span data-stu-id="68558-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="68558-107">Если пересылка блокируется, убедитесь, что она настроена на включение внешнего прямого перенаправления.</span><span class="sxs-lookup"><span data-stu-id="68558-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="68558-108">Вы можете проверить политику фильтрации исходящих сообщений в центре безопасности и соответствия требованиям или выполнив команду Get – Хостедаутбаундспамфилтерполици | FL Name, Аутофорвардингмоде.</span><span class="sxs-lookup"><span data-stu-id="68558-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="68558-109">Если вы хотите настроить блокировку с пересылкой, то та же команда сообщит вам о состоянии политики сейчас.</span><span class="sxs-lookup"><span data-stu-id="68558-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="68558-110">Примечание: в политике фильтрации нежелательной почты по умолчанию рекомендуется оставить внешнюю пересылку отключенной и включить ее только для тех пользователей, которым требуется внешняя переадресация, создав пользовательскую политику для этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="68558-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="68558-111">Дополнительные сведения можно узнать в статье [Настройка переадресации внешних сообщений электронной почты в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="68558-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>