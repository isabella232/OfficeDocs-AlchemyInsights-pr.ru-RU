---
title: 2419 — не удается включить аудит
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767612"
---
# <a name="unable-to-enable-unified-auditing"></a>Не удается включить единый аудит

При попытке включить единый аудит для организации может появиться сообщение об ошибке, похожее на следующее:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Чтобы устранить эту проблему, выполните указанные ниже действия.

1. [Подключитесь к Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Выполните следующий командлет:

   ```
   Enable-OrganizationCustomization
   ```

3. Подождите в течение 60 минут, пока предыдущее значение не вступит в силу.

4. Выполните следующую команду в Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Дополнительные сведения можно найти в следующих статьях:

- [Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Включение и отключение поиска в журнале аудита](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
