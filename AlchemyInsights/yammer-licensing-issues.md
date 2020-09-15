---
title: Проблемы с лицензированием Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657289"
---
# <a name="yammer-licensing-issues"></a>Проблемы с лицензированием Yammer

У всех пользователей должна быть лицензия для применения службы Yammer корпоративный, но по умолчанию Yammer не требует наличия лицензии на доступ к службе. Если администратор изменит этот параметр, чтобы заблокировать пользователей Microsoft 365 без лицензии Yammer, пользователи, которым не назначена лицензия Yammer корпоративный, не смогут получить доступ к службе Yammer. Дополнительные сведения см. в статье [Управление лицензиями пользователей Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365). 

При удалении лицензий пользователей плитка Yammer больше не отображается, а другие службы могут скрыть функции путем удаления лицензии. В других случаях функции могут по-прежнему отображаться, но для работы потребуется назначить лицензию.  

**Лицензия для пользователя не обновляется**  

Иногда пользователь, которому назначена лицензия, не может получить доступ к Yammer. Чаще всего задержки возникают в процессе массового назначения лицензий. Обновление пользователей Yammer может происходить не в том же порядке, в котором меняются лицензии в Azure AD, так как система работает асинхронно. Подождите до 24 часов, прежде чем сообщать в службу поддержки о проблемах с синхронизацией лицензий.  

**Массовое назначение лицензий**  

Лицензии можно назначать через центр администрирования или сценарии PowerShell. Дополнительные сведения см. в статьях [Назначение лицензий пользователям](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и [Назначение лицензий для учетных записей пользователей с помощью PowerShell в Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Служба поддержки Майкрософт не предоставляет помощь в создании сценариев, но документация по назначению лицензий Yammer доступна. Дополнительные сведения см. в статье [Управление лицензиями Yammer с помощью Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).