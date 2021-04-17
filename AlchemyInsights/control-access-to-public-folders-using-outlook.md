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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816753"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Управление доступом к общедоступным папкам с помощью Outlook

Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.

1. Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook  
$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook. Это значение используется по умолчанию.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows. Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.

Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).
