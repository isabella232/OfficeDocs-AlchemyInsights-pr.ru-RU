---
title: Импорт и экспорт из Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898050"
---
# <a name="import-and-export-from-yammer"></a>Импорт и экспорт из Yammer

**Импорт**

Возможности импорта пользователей зависят от того, находится ли сеть Yammer в [основном режиме для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) или нет.

- **Неосновной режим.** Пользователей можно импортировать в группы с помощью функции [Добавить из адресной книги](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (не более 100 пользователей) в окне параметров группы или в сеть с помощью [массового обновления](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в Администраторе сети.
- **Основной режим.** Операции членства в группах и членства в сети следует выполнять на [портале администрирования Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [портале Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) или с помощью других функций Azure AD. Сети в основном режиме больше не имеют доступа к массовому обновлению и другим устаревшим функциям.

> [!IMPORTANT]
> В Yammer никогда не было возможности импорта содержимого из Администратора сети, даже если в другой сети использовалась функция экспорта данных. Возможна повторная публикация контента с помощью решений партнеров или API Yammer REST.

**Экспорт**

[Функция экспорта сетевых данных в Администраторе сети](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) позволяет экспортировать контент из сетей Yammer, включая сообщения и файлы. Вложения могут быть очень большими, что потребует продолжительного времени на выполнение экспорта. Рекомендуется экспортировать активные сети с помощью [API экспорта данных](https://developer.yammer.com/docs/data-export-api) блоками за день или за неделю. Служба поддержки Майкрософт не предлагает пользовательских сценариев для этой цели.

Имеется отдельная функция [экспорта GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) для экспорта контента отдельному пользователю.