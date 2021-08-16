---
title: Электронная почта рабочего процесса не отправляется
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072533"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Электронная почта рабочего процесса не отправляется для SharePoint или библиотеки

1. Электронная почта из рабочего процесса отправляется не всем пользователям или только конкретным пользователям, или вы видите ошибку Сообщение электронной почты не может быть **отправлено. Убедитесь,** что у электронной почты есть допустимый получатель .

    Проверьте, существует ли пользователь в группе **разрешений "Все** люди" (список сведений о пользователе) для этой коллекции сайтов.  Пример прямого URL-адреса: <tenant> https:// .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Если пользователя не существует, убедитесь, что пользователь подписан на страницу. 
    - Если это внешний пользователь, убедитесь, что приглашение было принято.
    - Если пользователь существует в группе разрешений, убедитесь, что адрес электронной почты правильный.
    - Если адрес электронной почты пользователей здесь не установлен, создайте образец оповещения для этого пользователя, который заставляет синхронизировать эту учетную запись пользователя из профилей пользователей SharePoint в эту коллекцию сайтов.
 
2. Электронная почта из рабочего процесса отправляется администраторам коллекции сайтов, но не другим пользователям и см. ошибку HTTP Запрещено **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    См. статью Отказано в доступе при отправке электронной почты [в группу SharePoint.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Кроме того, убедитесь, **что** функция блокировки режима блокировки сайта с ограниченным доступом пользователя не активна.


## <a name="related-topics"></a>Похожие темы
Хотите попробовать Microsoft Flow в SharePoint Online?
- [Создание Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


