---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406601"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Управление доступом к общедоступным папкам с помощью Outlook

Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.

1. Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows. Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.

Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).
