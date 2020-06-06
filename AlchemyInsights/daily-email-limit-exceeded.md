---
title: Превышен ежедневный лимит электронной почты. Рабочий процесс приостановлен.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580346"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Превышен ежедневный лимит электронной почты. Рабочий процесс приостановлен.

Эту ошибку можно получить в следующих сценариях:

- В SharePoint Online есть рабочий процесс, в котором используется тип платформы рабочих процессов SharePoint 2010 или SharePoint 2013.
- Рабочий процесс настроен на отправку настраиваемого сообщения электронной почты более чем 200 пользователям одновременно, более чем 10 000 получателей в день или более 30 сообщений в минуту.
- При запуске рабочего процесса сообщение электронной почты не отправляется и обратите внимание на следующее поведение:
    - Для рабочего процесса, использующего тип платформы SharePoint 2013, перейдите на страницу **состояния рабочего процесса** . На странице "состояние рабочего процесса" для параметра **внутренний статус** задано значение **начато**, а всплывающая подсказка **не может быть отправлена получателю**.

Чтобы обойти эту проблему, настройте рабочий процесс на отправку сообщений электронной почты без превышения ограничения на количество [отправителей в Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например, используйте приостановку в рабочем процессе, отправьте сообщение электронной почты в группу Microsoft 365, группу рассылки или группу безопасности с включенной поддержкой почты или отправьте сообщение менее чем 200 получателям за раз.


Более подробную информацию можно найти в следующей [статье](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Связанные статьи
- [Создание последовательности](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 