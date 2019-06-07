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
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755050"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Определение активности правила для папки "Входящие" в журналах аудита

Вы можете использовать поиск в журнале аудита в центре безопасности & соответствия требованиям для просмотра событий правил папки "Входящие" (создание, изменение и удаление правил для папки "Входящие").

1. Вход в [центр соответствия требованиям & безопасности Office 365](https://protection.office.com/)

2. Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.

3. Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .

4. В разделе **действия почтового ящика Exchange**убедитесь, что для поля **действия** задано значение создать, **InboxRule создать/изменить/включить или отключить правило для папки "Входящие"**.

5. Нажмите кнопку **Поиск**.

В списке результатов выберите запись аудита. В всплывающем меню сведения щелкните **Дополнительные сведения**. Сведения о параметрах правила папки "Входящие" отображаются в поле **Параметры** .

Дополнительные сведения см. в статье [Определение, создал ли пользователь правило для папки "Входящие"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
