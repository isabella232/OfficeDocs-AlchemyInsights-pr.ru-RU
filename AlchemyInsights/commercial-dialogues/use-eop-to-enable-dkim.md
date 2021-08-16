---
title: Используйте Exchange Online PowerShell, чтобы включить DKIM для определенного домена
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070326"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Используйте Exchange Online PowerShell, чтобы включить DKIM для определенного домена

Если вы не можете создать записи DKIM DNS в центре администрирования, попробуйте использовать Exchange Online PowerShell. 

Чтобы создать запись DKIM DNS с Exchange Online PowerShell, выполните следующие действия:

1. Откройте Windows PowerShell администратора и запустите следующие команды в описанной последовательности:

    а. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Если у вас возникли проблемы с подключением Exchange Online PowerShell, [Подключение в Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. После подключения к Exchange Online PowerShell запустите следующую команду:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. После успешного выполнения вышеуказанной команды запустите следующую команду, чтобы завершить сеанс Exchange Online PowerShell:

    `Remove-PSSession $Session` 



