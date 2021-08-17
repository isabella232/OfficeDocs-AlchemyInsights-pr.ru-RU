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
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107155"
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