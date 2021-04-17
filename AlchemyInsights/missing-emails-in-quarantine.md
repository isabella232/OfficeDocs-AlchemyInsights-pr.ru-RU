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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831747"
---
# <a name="missing-emails-in-quarantine"></a>Отсутствующие сообщения электронной почты в карантине"

Администраторы могут [просматривать, выпускать или удалять эти сообщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Чтобы открыть Центр & безопасности, перейдите в [https://protection.office.com](https://protection.office.com/) . Чтобы открыть страницу карантина напрямую, перейдите к [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Вы можете искать по следующим значениям:  

- **Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения. Если выбрать сообщение в списке, значение **ID**  сообщения появится в области сведений, которая отображается. Администраторы могут использовать [трассировку сообщений](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) для поиска сообщений и соответствующих им значений идентификатора сообщения.
- **Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.
- **Адрес электронной почты получателя**: адрес электронной почты одного получателя.
- **Тема**: Используйте всю тему сообщения. При поиске регистр не учитывается.

После того как вы ввели критерии поиска, нажмите кнопку ![ Обновить ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **обновление,** чтобы отфильтровать результаты.  

Для просмотра и управления сообщениями и файлами в карантине используются такие коды, как:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage.](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обратите внимание, что этот командлет только для сообщений, а не файлов вредоносных программ из ATP для SharePoint Online, OneDrive для бизнеса или Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)