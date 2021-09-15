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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327827"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Отчеты в Центре администрирования Microsoft 365 не отображают понятное имя пользователя

Отчеты в Центре администрирования Microsoft 365 не отображают имена пользователей. Вместо этого они содержат буквенное-числовые значения, например B2BC6C15BB9FCDEA71E5CD302D228CC8.

Это ожидаемое поведение, о котором было уведомлено в Центре сообщений (MC275344, опубликовано 3 августа 2021 г.). 

Глобальные администраторы могут отменить это изменение в своем клиенте и отображать идентифицируемые сведения пользователей, если это разрешено политиками конфиденциальности организации. Чтобы отменить изменение в клиенте:

1. В Центре администрирования выберите **Параметры** > **Параметры организации** > [**Службы**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) и нажмите **Отчеты**. 
1. В разделе **Выберите способ отображения сведений о пользователе** нажмите **Показывать персональные сведения пользователя в отчетах** и повторно запустите отчет.