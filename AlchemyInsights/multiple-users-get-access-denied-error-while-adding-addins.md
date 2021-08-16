---
title: Ошибка "Отказано в доступе" для нескольких пользователей при добавлении надстроек в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065405"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Ошибка "Отказано в доступе" для нескольких пользователей при добавлении надстроек в Outlook

Вы можете указать, каким администраторам в вашей организации разрешается устанавливать надстройки для Outlook и управлять ими. Кроме того, можно указать, каким пользователям в организации будет разрешено устанавливать надстройки и управлять ими для собственных нужд.

Подробные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Чтобы убедиться в том, что вы назначили разрешения для пользователя, замените <Role Name> на название проверяемой роли и выполните следующую команду в Exchange Online PowerShell:

Get-ManagementRoleAssignment -Роль "<Role Name>" -GetEffectiveUsers

В этом примере показано, как проверить, кому назначены разрешения на установку в организации надстроек из Магазина Office.

PowerShell

-Роль "Приложения Org Marketplace" -GetEffectiveUsers

В результатах Get-ManagementRoleAssignment просмотрите записи в столбце "Действующие пользователи".

Дополнительные сведения о синтаксисе и параметрах см. в разделе [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 