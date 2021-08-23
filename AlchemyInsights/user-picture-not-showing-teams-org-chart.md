---
title: Изображение пользователя не отображается в организационной диаграмме Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467380"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Изображение пользователя не отображается в организационной диаграмме Microsoft Teams

Если у одного или нескольких сотрудников вашей организации отсутствует фотография профиля в организационной диаграмме, возможно, для параметра **ShowInAddressLists** установлено значение **False**:

1. Перейдите в Центр администрирования Microsoft 365 > [**Активные пользователи**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) и выберите пользователя с отсутствующей фотографией. 
1. Выберите вкладку **Почта** и убедитесь, что для параметра **Показать в глобальном списке адресов** значение **Да**. 

Если установка для параметра **ShowInAddressLists** значения **Да** не работает, проверьте следующее:

- Пользователь может быть скрыт из списка получателей в Exchange. Дополнительные сведения см. в разделе [Управление списками адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Пользователь может быть скрыт из списка адресов в Azure Active Directory. Дополнительные сведения см. в разделе [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
