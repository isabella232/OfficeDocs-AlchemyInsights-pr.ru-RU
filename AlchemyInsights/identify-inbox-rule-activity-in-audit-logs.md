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
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331136"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Определение активности правил "Входящие" в журналах аудита

Вы можете использовать поиск журнала аудита в Центр соответствия требованиям Microsoft 365 для просмотра событий правил "Входящие" (создание, изменение и удаление правил входящих).

1. Выполните одно из следующих действий:
   - В Центр соответствия требованиям Microsoft 365 <https://compliance.microsoft.com> , перейдите к **решений** \> **аудита**. Или, чтобы перейти непосредственно на страницу **Аудит,** используйте <https://compliance.microsoft.com/auditlogsearch> .
   - На портале Microsoft 365 Defender <https://security.microsoft.com> на сайте , перейдите к **аудиту**. Или, чтобы перейти непосредственно на страницу **Аудит,** используйте <https://security.microsoft.com/auditlogsearch> .

2. На **вкладке Поиск** на странице **Аудит** настройте следующие параметры:
   - **Диапазон дат и** времени. Выберите диапазон даты и времени в **полях "Начните"** **и "Конец".**
   - **Действия:** Выберите одно или несколько следующих значений:
     - **Правило создания почтовых ящиков New-InboxRule из Outlook Web App**
     - **Правило Изменить set-InboxRule из Outlook Web App**.
     - **Обновление правил почтового ящика Outlook клиента**

3. Когда вы закончите, нажмите кнопку **Поиск**. Действия отображаются на новой странице **поиска аудита.**

4. Выберите действие в результатах, чтобы открыть вылет сведений. Сведения о параметрах правил "Входящие" отображаются в поле **Параметры.**

Дополнительные сведения см. в статью Определение, создал ли пользователь [правило "Входящие".](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
