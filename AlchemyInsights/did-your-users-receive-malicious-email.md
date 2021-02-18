---
title: Ваши пользователи получили вредоносное сообщение электронной почты?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291805"
---
# <a name="did-your-users-receive-malicious-email"></a>Ваши пользователи получили вредоносное сообщение электронной почты?

- Теперь вы можете сообщить о вредоносном сообщении в корпорацию Майкрософт с помощью [Отправки администратора в Центре безопасности и соответствия требованиям](https://sip.protection.office.com/reportsubmission).

Сообщения, отправленные с помощью [отправки администратора](https://sip.protection.office.com/reportsubmission), и во всплывающем окне **сведений** отображаются следующие результаты:

- Возникновение сбоя при проверке подлинности электронной почты отправителя в момент доставки.
- Сведения о любых совпадениях политик, которые могут повлиять на решение по безопасности касательно сообщения или переопределить его.
- Текущие результаты отключения, чтобы определить, были ли URL-адреса или файлы, содержащиеся в сообщении, вредоносными или нет.
- Отзывы оценщиков

Если было обнаружено переопределение, повторное сканирование должно завершиться через несколько минут. Если проблема не связана с проверкой подлинности электронной почты или переопределение не повлияло на доставку, то обратная связь оценщиков может занять до суток.

Если вы не согласны с конечным решением по безопасности касательно сообщения, URL-адреса или файла (заблокированных или не заблокированных), отправьте сообщение через день после повторного сканирования. Очень высокая вероятность того, что решение по безопасности изменится после повторной отправки сообщения.

В то же время вы можете удалить вредоносную электронную почту из пользовательских папок "Входящие", следуя инструкциям, в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Пользователи с Microsoft Defender для Office 365 могут:
    - использовать [обозреватель угроз для поиска и удаления подозрительных сообщений электронной почты](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [использовать Безопасные ссылки, чтобы заблокировать доступ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) к вредоносному URL-адресу.
    - отслеживать пользователей, нажимавших на вредоносные URL-адреса и получивших к ним доступ. [Просмотр фишингового URL-адреса и нажатие на сведенья о решении по безопасности](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Получение-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - вручную [начать автоматическое исследование](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Также вы можете создать защиту от вредоносных файлов и URL-адресов, следуя инструкциям в статье [Защита от вредоносных URL-адресов и файлов](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).