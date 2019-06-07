---
title: Устранение проблем с установкой DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765351"
---
# <a name="fix-dkim-setup-issues"></a>Устранение проблем с установкой DKIM

Если у вас возникли проблемы, связанные с включением DKIM для вашего личного домена, выполните указанные ниже действия.

- Большинство проблем с установкой DKIM связаны с неверными записями DNS. Убедитесь, что запись CNAME DKIM (а**не** запись TXT) отформатирована правильно. Дополнительные сведения см. в этой [статье](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- После создания или обновления DNS-записей DKIM в службе хостинга DNS для вашего домена (как правило, регистратора доменных имен) Дождитесь распространения записей DNS.

- Если вы не можете создавать записи DNS DKIM в центре администрирования, вы можете \<заменить кустомдомаин\> на свой личный домен (например, contoso.com) и выполнить эту команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
