---
title: Ваши пользователи получили вредоносное сообщение электронной почты?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326719"
---
# <a name="did-your-users-receive-malicious-email"></a>Ваши пользователи получили вредоносное сообщение электронной почты?

Теперь вы можете сообщать о вредоносных сообщениях в корпорацию Майкрософт с помощью функции [Отправки в Центре Microsoft 365 Defender](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Сообщения, отправленные в разделе [Отправки администратора](https://security.microsoft.com/reportsubmission?viewid=admin), проверяются, и во всплывающем окне сведений выводятся следующие результаты:

- Возникновение сбоя при проверке подлинности электронной почты отправителя в момент доставки.
- Сведения о любых совпадениях политик, которые могут повлиять на решение по безопасности касательно сообщения или переопределить его.
- Текущие результаты отключения, чтобы определить, были ли URL-адреса или файлы, содержащиеся в сообщении, вредоносными или нет.
- Отзывы оценщиков

Если обнаружено переопределение, повторная проверка завершится через несколько минут. Если проблема не связана с проверкой подлинности электронной почты или доставка не подверглась действию переопределения, получение обратной связи от оценщиков может занять до суток.

Если вы не согласны с конечным решением по безопасности касательно сообщения, URL-адреса или файла (заблокированных или не заблокированных), отправьте сообщение через день после повторного сканирования. Очень высокая вероятность того, что решение по безопасности изменится после повторной отправки сообщения.

В то же время вы можете удалить вредоносную электронную почту из пользовательских папок "Входящие", следуя инструкциям, в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Пользователи с Microsoft Defender для Office 365 могут:
  - использовать [обозреватель угроз для поиска и удаления подозрительных сообщений электронной почты](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [использовать Безопасные ссылки, чтобы заблокировать доступ](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) к вредоносному URL-адресу.
  - отслеживать пользователей, нажимавших на вредоносные URL-адреса и получивших к ним доступ. [Просмотрите фишинговые URL-адреса и щелкните ](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Получение-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace), чтобы получить решение
  - вручную [начать автоматическое исследование](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Также вы можете создать защиту от вредоносных файлов и URL-адресов, следуя инструкциям в статье [Защита от вредоносных URL-адресов и файлов](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
