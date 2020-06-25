---
title: Использование PowerShell для политик общего доступа и связей организации
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854035"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Использование PowerShell для политик общего доступа и связей организации


Для связей организации ознакомьтесь с подробным синтаксисом и сведениями о параметрах для: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) и [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Чтобы создать политику общего доступа, используйте [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Чтобы [применить политику общего доступа к почтовому ящику или пользователю](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), вам потребуется использовать сочетание командлетов [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) и [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) с созданной политикой. Чтобы [изменить, отключить или удалить политику общего доступа](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), вам потребуется использовать [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) и [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Полные сведения по этой теме см. в статье:**

[Общий доступ в Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)