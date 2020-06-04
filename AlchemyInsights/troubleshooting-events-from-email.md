---
title: Устранение неполадок с событиями на основе электронной почты
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44515988"
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