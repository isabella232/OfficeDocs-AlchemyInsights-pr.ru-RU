---
title: Установите значение ClientAccessServerEnabled для True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737693"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Установите значение ClientAccessServerEnabled для True

Если вы не можете открыть зашифрованное сообщение электронной почты и вместо этого увидеть вложение **rpmsg,** выполните следующие действия:

1. Подключитесь к Exchange Online PowerShell.

> [!NOTE]
> Чтобы подключиться к Exchange Online PowerShell, необходимо войти с помощью учетной записи глобального администратора или администратора Exchange.

   а. Откройте Windows PowerShell, а затем запустите следующую команду: `$UserCredential = Get-Credential`
б. В **диалоговом окне Windows PowerShell запроса** учетных данных введите свою учетную запись или учетную запись школы и пароль c. Нажмите **ОК**. 

2. Запустите следующую команду, чтобы создать новый сеанс:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    а. Выполните следующую команду:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Запустите `Get-IRMConfiguration` команду.

4. Проверьте параметр **ClientAccessServerEnabled.** 

    а. Если **параметр ClientAccessServerEnabled** настроен на **False,** запустите следующий cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Всегда закройте сеанс powershell следующей командой: `Remove-PSSession $Session`

Дополнительные сведения см. в [веб-сайте Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

