---
title: Удаление корневого сайта SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815484"
---
# <a name="delete-the-sharepoint-root-site"></a>Удаление корневого сайта SharePoint

Удаление корневого сайта SharePoint **не поддерживается**.

1.  Если корневой сайт уже удален, при попытке получить доступ к сайту пользователи увидят сообщение об ошибке 404, "Файл не найден".
2.  Чтобы устранить эту проблему, восстановите сайт в новом центре администрирования SharePoint. Для этого на странице [Удаленные сайты](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) выберите корневой сайт и нажмите кнопку "Восстановить".
3.  После восстановления корневого сайта вместо того, чтобы удалять его, используйте функцию [замены сайта](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) в новом центре администрирования SharePoint.

Дополнительную информацию см. в статье [Модернизация корневого сайта](https://docs.microsoft.com/sharepoint/modern-root-site).