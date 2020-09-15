---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680489"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Управление доступом к общедоступным папкам с помощью Outlook

Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.

1. Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows. Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.

Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).
