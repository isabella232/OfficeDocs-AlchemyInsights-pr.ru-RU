---
title: Параметры SMTP для почтовой службы Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 261695a0bf736a51514df50c0ad66aaab5b50edb
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603299"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Параметры SMTP для почтовой службы Microsoft 365

Параметры SMTP для почтовых служб Microsoft 365:

**Сервер**: smtp.office365.com </br>
**Порт**: 587 </br>
**Шифрование**: STARTTLS (сейчас поддерживается только версия TLS 1.2. Убедитесь, что ваше приложение или устройство поддерживает TLS 1.2) </br>
**Имя пользователя**: ваш адрес Office 365 (например, proverka@yourdomain.com) </br>
**Пароль**: ваш пароль Office 365 </br>
**Проверка подлинности**: требуется </br>
**Ограничения на отправку**: 10 000 писем в день </br>

Параметры POP и IMAP см. в статье [Параметры POP, IMAP и SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Сведения о вариантах ретрансляции почты с помощью Microsoft 365 и инструкции см. в статье [Настройка многофункционального устройства или приложения для отправки электронной почты с помощью Microsoft 365 или Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).