---
title: Устранение проблем установки DKIM
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945944"
---
# <a name="fix-dkim-setup-issues"></a>Устранение проблем установки DKIM

Если у вас проблемы с включением DKIM для настраиваемого домена, используйте следующие действия:

- Большинство проблем установки DKIM связаны с неправильными записями DNS. Убедитесь, что запись DKIM CNAME **(а** не запись TXT) отформатирована правильно. Дополнительные сведения см. в этом [разделе.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- После создания или обновления записей DKIM DNS в службе размещения DNS для домена (как правило, регистратора домена) дождись распространения записей DNS.

- Если вы не можете создать записи DKIM DNS в центре администрирования, вы можете заменить пользовательский домен (например, contoso.com) и запустить эту команду в \<CustomDomain\> [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
