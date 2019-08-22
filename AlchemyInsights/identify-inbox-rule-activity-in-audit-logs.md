---
title: Определение активности правила для папки "Входящие" в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539186"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Определение активности правила для папки "Входящие" в журналах аудита

Вы можете использовать поиск в журнале аудита в центре безопасности & безопасности Office 365 для просмотра событий правил папки "Входящие" (создание, изменение и удаление правил для папки "Входящие").

1. Войдите в [центр соответствия требованиям & безопасности Office 365](https://protection.office.com/).

2. Перейдите на страницу **** > **поиска журнала аудита** поиска.

3. Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .

4. В разделе **действия почтового ящика Exchange**убедитесь, что для поля **действия** задано значение создать, **InboxRule создать/изменить/включить или отключить правило для папки "Входящие"**.

5. Нажмите кнопку **Поиск**.

В списке результатов выберите запись аудита. В всплывающем меню сведения щелкните **Дополнительные сведения**. Сведения о параметрах правила папки "Входящие" отображаются в поле **Параметры** .

Дополнительные сведения см. в статье [Определение, создал ли пользователь правило для папки "Входящие"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
