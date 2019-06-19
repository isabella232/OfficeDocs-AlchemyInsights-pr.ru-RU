---
title: 2419 — не удается включить аудит
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065693"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="f641d-102">Не удается включить единый аудит</span><span class="sxs-lookup"><span data-stu-id="f641d-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="f641d-103">При попытке включить единый аудит для организации Office 365 может появиться сообщение об ошибке, похожее на следующее:</span><span class="sxs-lookup"><span data-stu-id="f641d-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="f641d-104">Чтобы устранить эту проблему, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="f641d-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="f641d-105">[Подключитесь к Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="f641d-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="f641d-106">Выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="f641d-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="f641d-107">Подождите в течение 60 минут, пока предыдущее значение не вступит в силу.</span><span class="sxs-lookup"><span data-stu-id="f641d-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="f641d-108">Выполните следующую команду в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f641d-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="f641d-109">Дополнительные сведения можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="f641d-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="f641d-110">Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f641d-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="f641d-111">Включение и отключение поиска в журнале аудита Office 365</span><span class="sxs-lookup"><span data-stu-id="f641d-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
