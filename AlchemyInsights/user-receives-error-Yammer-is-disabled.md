---
title: Пользователь получил сообщение об ошибке AADSTS7000112 "Yammer отключен"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: f2e23d63338ece5332ad4fd2b2d59021eb45d9bf32632d3cc23089c919d4e402
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971244"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Пользователь получил сообщение об ошибке AADSTS7000112 "Yammer отключен"

Если появляется сообщение об ошибке "AADSTS7000112: Приложение '00000005-0000-0ff1-ce00-000000000000'(Yammer) отключено", это значит, что в субъекте-службе внутри Azure AD возникла проблема. Администратор мог отключить субъект-службу, чтобы заблокировать доступ к Yammer.

Отключение субъекта-службы не рекомендуется, это может привести к возникновению дополнительных проблем. Подробнее о поддерживаемых способах блокирования доступа пользователей к Yammer см. в статье [Отключение доступа к Yammer для пользователей Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Чтобы устранить эту ошибку на портале Azure и восстановить доступ пользователей к Yammer, выполните указанные ниже действия.

1.  Откройте страницу Azure Active Directory и на панели навигации слева выберите **Корпоративные приложения** из раздела **Управление**.
3.  В поле поиска введите **Office 365 Yammer** и выберите имя приложения, чтобы открыть параметры.
4.  Нажмите кнопку **Свойства** в разделе **Управление** на панели навигации слева.
5.  Установите для параметра **Разрешать вход пользователям?** значение **Да**, а затем нажмите **Сохранить**.
6.  Повторно войдите в Yammer Вам может понадобиться удалить файлы cookie.

Вместо этого для установки значения можно выполнить команду PowerShell. Подробнее см. в статье [Ошибка "При выполнении входа возникла проблема" при нажатии на плитку Yammer в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 