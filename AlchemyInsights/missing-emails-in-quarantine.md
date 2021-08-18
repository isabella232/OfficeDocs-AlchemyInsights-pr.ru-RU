---
title: Отсутствующие сообщения электронной почты в карантине
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329675"
---
# <a name="missing-emails-in-quarantine"></a>Отсутствующие сообщения электронной почты в карантине

Администраторы могут [просматривать, выпускать или удалять эти сообщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

На портале <https://security.microsoft.com> Microsoft 365 Defender, перейдите на  \> **карантин** Review . Или, чтобы перейти непосредственно на страницу **Карантина,** используйте <https://security.microsoft.com/quarantine> .  

Дополнительные сведения о значениях поиска и фильтрации, которые можно использовать, см. в статью Управление карантинными сообщениями и файлами в качестве администратора [в EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Для просмотра и управления сообщениями и файлами в карантине используются такие коды, как:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обратите внимание, что этот комлет только для сообщений, а не файлов из Сейф Вложения для SharePoint, OneDrive или Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
