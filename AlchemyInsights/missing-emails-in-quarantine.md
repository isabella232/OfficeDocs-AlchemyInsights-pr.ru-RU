---
title: Отсутствующие сообщения электронной почты в карантине
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673727"
---
# <a name="missing-emails-in-quarantine"></a>Отсутствующие сообщения электронной почты в карантине "

Администраторы могут [просматривать, освобождать или удалять эти сообщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Чтобы открыть центр безопасности & соответствия требованиям, перейдите на страницу [https://protection.office.com](https://protection.office.com/) . Чтобы напрямую открыть страницу карантина, перейдите на страницу [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Вы можете искать по следующим значениям:  

- **Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения. Если в списке выбрано сообщение, в появившейся всплывающей области **сведения** отображается значение **идентификатора сообщения** . Администраторы могут использовать [трассировку сообщений](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) для поиска сообщений и соответствующих им значений идентификатора сообщения.
- **Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.
- **Адрес электронной почты получателя**: адрес электронной почты одного получателя.
- **Тема**: Используйте всю тему сообщения. При поиске регистр не учитывается.

После ввода условий поиска нажмите кнопку ![ Обновить кнопку обновить, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** чтобы отфильтровать результаты.  

Для просмотра и управления сообщениями и файлами в карантине используются следующие командлеты:
- [Delete — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Обратите внимание, что этот командлет предназначен только для сообщений, а не от вредоносных файлов из ATP для SharePoint Online, OneDrive для бизнеса или Teams.
- [Release — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)