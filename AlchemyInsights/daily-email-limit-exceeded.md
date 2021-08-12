---
title: Превышено ежедневное ограничение электронной почты. Рабочий процесс приостановлен.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914664"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Превышено ежедневное ограничение электронной почты. Рабочий процесс приостановлен.

Эта ошибка может быть получена в следующих сценариях:

- Рабочий процесс в SharePoint Online, использующий тип платформы SharePoint 2010 или SharePoint 2013 года.
- Рабочий процесс настроен для отправки настраиваемой электронной почты более чем 200 пользователям одновременно, более 10 000 получателей в день или более 30 сообщений в минуту.
- При запуске рабочего процесса сообщение электронной почты не отправляется, и вы заметите следующее поведение:
    - Для рабочего процесса с SharePoint типа платформы 2013 вы можете просмотреть страницу **Состояние рабочего** процесса. На странице Состояние рабочего процесса  для внутреннего состояния установлено **начало,** а на информационном шаре отображается не удается отправить **получателю**.

Чтобы решить эту проблему, настройте рабочий процесс для отправки сообщений электронной почты, не превышая Exchange Online [отправитель.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Например, используйте паузу в рабочего процесса, отправьте сообщение в группу Microsoft 365, группу рассылки или группу безопасности с включенной почтой или отправьте сообщение менее чем 200 получателям одновременно.


Дополнительные сведения см. в следующей [статье](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Похожие темы
- [Создание Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 