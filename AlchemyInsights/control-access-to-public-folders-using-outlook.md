---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032571"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Управление доступом к общедоступным папкам с помощью Outlook

Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.

1. Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows. Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.

Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).
