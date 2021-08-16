---
title: Назначение роли журнала аудита в Центре безопасности и соответствия требованиям Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 5ddfda8687fe3ae2467ad221c7c083f46239826e23b10b91732ea06fd4649f3e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006183"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Назначение роли журнала аудита в Центре безопасности и соответствия требованиям Office 365

Для поиска по журналу аудита Office 365 администратору должна быть назначена роль **Только просмотр журналов аудита** или **Журналы аудита** в Exchange Online. Эти роли назначены группам ролей "Управление соответствием" и "Управление организацией" по умолчанию. Глобальные администраторы в Office 365 и Microsoft 365 автоматически добавляются в качестве участников группы ролей "Управление организацией".

Чтобы разрешить пользователю выполнять поиск с минимальным уровнем привилегий, создайте пользовательскую группу ролей в Exchange Online, добавьте роль **Только просмотр журналов аудита** или **Журналы аудита**, а затем добавьте пользователя в качестве участника новой группы ролей.

Дополнительные сведения см. в статьях [Управление группами ролей в Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) и [Поиск по журналу аудита в Центре безопасности и соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).