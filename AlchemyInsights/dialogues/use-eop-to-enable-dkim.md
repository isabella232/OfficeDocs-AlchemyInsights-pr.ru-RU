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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500883"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Используйте Exchange Online PowerShell, чтобы включить DKIM для определенного домена

Если вы не можете создать записи DKIM DNS в центре администрирования, попробуйте использовать Exchange Online PowerShell. 

Чтобы создать DKIM-запись DNS с помощью Exchange Online PowerShell, выполните следующие действия:

1. Откройте Windows PowerShell администратора и запустите следующие команды в описанной последовательности:

    а. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    в. `Import-PSSession $Session -DisableNameChecking`
    
Если у вас возникли проблемы с подключением к Exchange Online PowerShell, см. в обзоре [Connect to Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. После подключения к Exchange Online PowerShell запустите следующую команду:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. После успешного выполнения вышеуказанной команды запустите следующую команду, чтобы завершить сеанс PowerShell Exchange Online:

    `Remove-PSSession $Session` 



