---
title: Удаление корневого сайта SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768456"
---
# <a name="delete-the-sharepoint-root-site"></a>Удаление корневого сайта SharePoint

Удаление корневого сайта SharePoint **не поддерживается.**

1.  Если корневой сайт уже удален, при попытке получить доступ к сайту пользователи увидят сообщение об ошибке 404, «Файл не найден».
2.  Чтобы устранить эту проблему, восстановите сайт в новом центре администрирования SharePoint. Для этого на странице [Удаленные сайты](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) выберите корневой сайт и нажмите кнопку «Восстановить».
3.  После восстановления корневого сайта впредь, вместо того чтобы удалять его, используйте функцию [замены сайта](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) в новом центре администрирования SharePoint.

Дополнительную информацию см. в статье [Модернизация корневого сайта](https://docs.microsoft.com/sharepoint/modern-root-site).