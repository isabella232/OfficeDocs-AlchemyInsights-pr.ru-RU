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
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510142"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="462cd-102">Назначение роли журнала аудита в Центре безопасности и соответствия требованиям Office 365</span><span class="sxs-lookup"><span data-stu-id="462cd-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="462cd-103">Для поиска по журналу аудита Office 365 администратору должна быть назначена роль **Только просмотр журналов аудита** или **Журналы аудита** в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="462cd-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="462cd-104">Эти роли назначены группам ролей "Управление соответствием" и "Управление организацией" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="462cd-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="462cd-105">Глобальные администраторы в Office 365 и Microsoft 365 автоматически добавляются в качестве участников группы ролей "Управление организацией".</span><span class="sxs-lookup"><span data-stu-id="462cd-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="462cd-106">Чтобы разрешить пользователю выполнять поиск с минимальным уровнем привилегий, создайте пользовательскую группу ролей в Exchange Online, добавьте роль **Только просмотр журналов аудита** или **Журналы аудита**, а затем добавьте пользователя в качестве участника новой группы ролей.</span><span class="sxs-lookup"><span data-stu-id="462cd-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="462cd-107">Дополнительные сведения см. в статьях [Управление группами ролей в Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) и [Поиск по журналу аудита в Центре безопасности и соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="462cd-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>