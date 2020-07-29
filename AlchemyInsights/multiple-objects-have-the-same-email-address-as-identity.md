---
title: Для нескольких объектов используется один и тот же адрес электронной почты, используемый для идентификации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431535"
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