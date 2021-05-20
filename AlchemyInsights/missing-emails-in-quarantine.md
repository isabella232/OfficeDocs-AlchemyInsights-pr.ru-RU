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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539837"
---
# <a name="missing-emails-in-quarantine"></a>Отсутствующие сообщения электронной почты в карантине"

Администраторы могут [просматривать, выпускать или удалять эти сообщения.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Чтобы открыть Центр & безопасности, перейдите в [https://protection.office.com](https://protection.office.com/) . Чтобы открыть страницу карантина напрямую, перейдите к [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Вы можете искать по следующим значениям:  

- **Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения. Если выбрать сообщение в списке, значение **ID**  сообщения появится в области сведений, которая отображается. Администраторы могут использовать [трассировку сообщений](/microsoft-365/security/office-365-security/message-trace-scc) для поиска сообщений и соответствующих им значений идентификатора сообщения.
- **Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.
- **Адрес электронной почты получателя**: адрес электронной почты одного получателя.
- **Тема**: Используйте всю тему сообщения. При поиске регистр не учитывается.

После того, как вы ввели критерии поиска, нажмите ![кнопку Обновить](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обновить**, чтобы обновить результаты.

Для просмотра и управления сообщениями и файлами в карантине используются такие коды, как:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Обратите внимание, что этот комлет только для сообщений, а не файлов вредоносных программ из Microsoft Defender для Office 365 для SharePoint Online, OneDrive для бизнеса или Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)