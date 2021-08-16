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
ms.openlocfilehash: 4965e38f69c9d7f3a5c1facd23a0ee487e499f55f5779672808a54b86c90aeaa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102277"
---
# <a name="delete-the-sharepoint-root-site"></a>Удаление корневого сайта SharePoint

Удаление корневого сайта SharePoint **не поддерживается**.

1.  Если корневой сайт уже удален, при попытке получить доступ к сайту пользователи увидят сообщение об ошибке 404, "Файл не найден".
2.  Чтобы устранить эту проблему, восстановите сайт в новом центре администрирования SharePoint. Для этого на странице [Удаленные сайты](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) выберите корневой сайт и нажмите кнопку "Восстановить".
3.  После восстановления корневого сайта вместо того, чтобы удалять его, используйте функцию [замены сайта](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) в новом центре администрирования SharePoint.

Дополнительную информацию см. в статье [Модернизация корневого сайта](https://docs.microsoft.com/sharepoint/modern-root-site).