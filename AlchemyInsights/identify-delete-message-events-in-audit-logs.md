---
title: Определение событий удаления сообщений в журналах аудита
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115661"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Журналы аудита удаленных сообщений электронной почты

Начиная с января 2019 г. Корпорация Майкрософт по умолчанию включит журнал аудита почтовых ящиков. В противном случае, чтобы просмотреть события удаления сообщений для определенного пользователя, необходимо вручную включить действия удаления для аудита. Если журнал аудита почтовых ящиков уже включен для организации или для конкретного пользователя, выполните следующие действия.

1. Войдите в [центр Microsoft 365 соответствия требованиям](https://protection.office.com/)

2. Щелкните **поиск и исследование** и выберите поиск журнала **аудита.**

3. Выберите диапазон дат в полях **Даты начала** и **даты окончания.** Укажите имя пользователя, которое необходимо исследовать (пользователь, удаливший элементы). В поле **Действия** выберите удаленные сообщения из папки **"Удаленные** элементы" и "Перенесенные" сообщения **в папку "Удаленные элементы".**

4. Нажмите кнопку **Поиск**.

В результатах выберите запись аудита. Подробнее об этом читайте в материале **"Дополнительные сведения".** Дополнительные сведения об удалении элемента (например, строке субъекта и расположении элемента при его удалении) отображаются в **поле AffectedItems.** Свойство **ClientInfoString** покажет, произошло ли удаление в Outlook, Outlook в Интернете (ранее известном как Outlook Web App) или любом другом устройстве.

Дополнительные сведения см. в сообщении Определение того, кто настроил отправку электронной почты [для почтового ящика.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Примечание.** Вы не можете получить удаленные элементы с помощью функции журнала аудита. Чтобы получить удаленные сообщения в Outlook в Интернете, см. в [Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
