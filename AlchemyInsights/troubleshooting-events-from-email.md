---
title: Устранение неполадок с событиями на основе электронной почты
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834852"
---
# <a name="troubleshooting-events-from-email"></a>Устранение неполадок с событиями на основе электронной почты

1. Убедитесь, что для почтового ящика включена функция: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Затем просмотрите журналы "События на основе электронной почты" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. В журналах "События на основе электронной почты" найдите InternetMessageId, соответствующий элементу в почтовом ящике.  

4. TrustScore определяет, будет добавлен элемент или нет. События добавляются только при условии TrustScore = "Trusted".

TrustScore определяется свойствами SPF, DKIM или DMARC, содержащимися в заголовке сообщения.

Чтобы просмотреть эти свойства:

**Классическое приложение Outlook**

- Откройте элемент
- "Файл -> Свойства -> Заголовки Интернета"

или

**MFCMapi**

- Перейдите к элементу в папке "Входящие"
- Найдите PR_TRANSPORT_MESSAGE_HEADERS_W

Эти свойства определяются и записываются во время транспортировки и маршрутизации. Для дальнейшего устранения неполадок могут потребоваться действия по поддержке транспорта, связанные со сбоями в SPF, DKIM или DMARC.