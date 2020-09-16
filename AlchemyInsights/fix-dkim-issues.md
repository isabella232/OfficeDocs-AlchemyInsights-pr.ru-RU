---
title: Устранение проблем с установкой DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744963"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="f7ba8-102">Устранение проблем с установкой DKIM</span><span class="sxs-lookup"><span data-stu-id="f7ba8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="f7ba8-103">Если у вас возникли проблемы, связанные с включением DKIM для вашего личного домена, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="f7ba8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="f7ba8-104">Большинство проблем с установкой DKIM связаны с неверными записями DNS.</span><span class="sxs-lookup"><span data-stu-id="f7ba8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="f7ba8-105">Убедитесь, что запись CNAME DKIM (а**не** запись TXT) отформатирована правильно.</span><span class="sxs-lookup"><span data-stu-id="f7ba8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="f7ba8-106">Дополнительные сведения см. в этой [статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="f7ba8-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="f7ba8-107">После создания или обновления DNS-записей DKIM в службе хостинга DNS для вашего домена (как правило, регистратора доменных имен) Дождитесь распространения записей DNS.</span><span class="sxs-lookup"><span data-stu-id="f7ba8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="f7ba8-108">Если вы не можете создавать записи DNS DKIM в центре администрирования, вы можете заменить \<CustomDomain\> его на настраиваемый домен (например, contoso.com) и выполнить следующую команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="f7ba8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
