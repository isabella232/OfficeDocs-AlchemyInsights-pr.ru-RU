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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478334"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="4c3f8-102">Блокировка или разблокировка переадресации электронной почты</span><span class="sxs-lookup"><span data-stu-id="4c3f8-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="4c3f8-103">Чтобы включить или отключить переадресацию электронной почты для определенного почтового ящика, ознакомьтесь со статьей [Настройка переадресации электронной почты](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="4c3f8-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="4c3f8-104">На уровне клиента управление внешней пересылкой выполняется с помощью политики исходящей нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="4c3f8-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="4c3f8-105">Вы можете проверить политику фильтрации исходящих сообщений в центре безопасности и соответствия требованиям [здесь](https://protection.office.com/antispam) или с помощью [команды Get – хостедаутбаундспамфилтерполици](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="4c3f8-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="4c3f8-106">Если вы получаете следующее сообщение об ошибке: **"550 5.7.520 отказано в доступе, ваша организация не поддерживает внешнюю переадресацию**, убедитесь, что она настроена на включение внешнего автоматического перенаправления.</span><span class="sxs-lookup"><span data-stu-id="4c3f8-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="4c3f8-107">**Примечание:** Рекомендуется оставить внешнюю пересылку отключенной в политике фильтрации нежелательной почты по умолчанию и включить ее только для тех пользователей, которым требуется внешняя переадресация, создав пользовательскую политику для этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c3f8-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="4c3f8-108">Дополнительные сведения можно узнать в статье [Настройка переадресации внешних сообщений электронной почты в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="4c3f8-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>