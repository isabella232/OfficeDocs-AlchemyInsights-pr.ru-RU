---
title: Определение активности правил "Входящие" в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976878"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Определение активности правил "Входящие" в журналах аудита

Вы можете использовать поиск журнала аудита в центре Microsoft 365 безопасности & для просмотра событий правил входящие (создание, изменение и удаление правил входящих).

1. Войдите в [центр Microsoft 365 соответствия](https://protection.office.com/)требованиям.

2. Перейдите на **страницу поиска**  >  **журнала аудита поиска.**

3. Выберите диапазон дат в полях **Даты начала** и **даты окончания.**

4. В **Exchange** действия почтовых ящиков убедитесь, что поле **Действия** задано правилу **New-InboxRule Create/modify/enable/disable inbox.**

5. Нажмите кнопку **Поиск**.

В результатах выберите запись аудита. Подробнее об этом читайте в материале **"Дополнительные сведения".** Сведения о параметрах правил "Входящие" отображаются в поле **Параметры.**

Дополнительные сведения см. в статью Определение, создал ли пользователь [правило "Входящие"](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
