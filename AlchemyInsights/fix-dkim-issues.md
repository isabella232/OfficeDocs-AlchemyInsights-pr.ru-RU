---
title: Устранение проблем с установкой DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717575"
---
# <a name="fix-dkim-setup-issues"></a>Устранение проблем с установкой DKIM

Если у вас возникли проблемы, связанные с включением DKIM для вашего личного домена, выполните указанные ниже действия.

- Большинство проблем с установкой DKIM связаны с неверными записями DNS. Убедитесь, что запись CNAME DKIM (а**не** запись TXT) отформатирована правильно. Дополнительные сведения см. в этой [статье](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- После создания или обновления DNS-записей DKIM в службе хостинга DNS для вашего домена (как правило, регистратора доменных имен) Дождитесь распространения записей DNS.

- Если вы не можете создавать записи DNS DKIM в центре администрирования, вы можете \<заменить кустомдомаин\> на свой личный домен (например, contoso.com) и выполнить эту команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
