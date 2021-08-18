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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320369"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Установите значение ClientAccessServerEnabled для True

Если вы не можете открыть зашифрованное сообщение электронной почты и вместо этого увидеть вложение **rpmsg,** выполните следующие действия:

1. Подключитесь к Exchange Online PowerShell.

    **Примечание.** Чтобы подключиться к Exchange Online PowerShell, необходимо войти с помощью учетной записи глобального администратора Exchange администратора.

   а. Откройте Windows PowerShell, а затем запустите следующую команду:`$UserCredential = Get-Credential`
   б. В **диалоговом окне Windows PowerShell запроса** учетных данных введите свою учетную запись или учетную запись школы и пароль c. Нажмите кнопку **ОК**. 

2. Запустите следующую команду, чтобы создать новый сеанс:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    а. Выполните следующую команду:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Запустите `Get-IRMConfiguration` команду.

4. Проверьте параметр **ClientAccessServerEnabled.** 

    а. Если **параметр ClientAccessServerEnabled** настроен на **False,** запустите следующий cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Совет.** Всегда закройте сеанс powershell следующей командой: `Remove-PSSession $Session`

Дополнительные сведения см. [в Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

