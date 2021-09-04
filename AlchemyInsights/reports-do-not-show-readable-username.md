---
title: Отчеты в Центре администрирования Microsoft 365 не отображают понятное имя пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896350"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Отчеты в Центре администрирования Microsoft 365 не отображают понятное имя пользователя

Отчеты в Центре администрирования Microsoft 365 не отображают имена пользователей. Вместо этого они содержат буквенное-числовые значения, например B2BC6C15BB9FCDEA71E5CD302D228CC8.

Это ожидаемое поведение, о котором было уведомлено в Центре сообщений (MC275344, опубликовано 3 августа 2021 г.). 

Глобальные администраторы могут отменить это изменение в своем клиенте и отображать идентифицируемые сведения пользователей, если это разрешено политиками конфиденциальности организации. Чтобы отменить изменение в клиенте:

1. В Центре администрирования выберите **Параметры** > **Параметры организации** > [**Службы**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services) и нажмите **Отчеты**. 
1. В разделе **Выберите способ отображения сведений о пользователе** нажмите **Показывать персональные сведения пользователя в отчетах** и повторно запустите отчет.