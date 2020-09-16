---
title: Для нескольких объектов используется один и тот же адрес электронной почты, используемый для идентификации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724628"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Для нескольких объектов используется один и тот же адрес электронной почты, используемый для идентификации

**Несколько объектов**

Одна из распространенных причин этой ошибки заключается в том, что не удается правильно маршрутизировать запрос Outlook Web Access в присутствии нескольких объектов, у которых есть один и тот же адрес электронной почты, используемый для идентификации. Чтобы найти эти объекты, выполните следующие команды:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Чтобы устранить эту проблему, удалите несколько объектов с одинаковым адресом электронной почты, используемым для идентификации, и убедитесь в том, что есть один объект с определенной электронной почтой и что его типом получателя является UserMailBox.

** Тот же адрес используется для пользовательского и корпоративного почтовых ящиков **

Другая причина заключается в том, что один и тот же адрес используется для пользовательского и корпоративного почтовых ящиков. В этом случае пользователь должен изменить свой основной псевдоним пользователя до тех пор, пока Cafe не поддержит такой сценарий. Это постоянная ошибка, которые не исчезает без вмешательства.

Дополнительные сведения см. в разделе [Изменить адрес электронной почты или номер телефона для вашей учетной записи Майкрософт](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).