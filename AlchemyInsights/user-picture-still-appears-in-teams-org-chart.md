---
title: Изображение пользователя по-прежнему отображается в организационной диаграмме Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334381"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Изображение пользователя по-прежнему отображается в организационной диаграмме Microsoft Teams

Если профили одного или нескольких сотрудников вашей организации были удалены или отключены, но их фотографии профиля в организационной диаграмме по-прежнему присутствуют, возможно, для параметра **ShowInAddressLists** установлено значение False: 

1. Перейдите в Центр администрирования Microsoft 365 > [Активные пользователи](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) и выберите пользователя, чья фотография по-прежнему присутствует. 
1. Выберите вкладку **Почта** и убедитесь, что для параметра **Показать в глобальном списке адресов** значение **Нет**.

Если установка для параметра **ShowInAddressLists** значения **Нет** не работает, проверьте следующее: 

- Пользователь может быть показан в списке получателей в Exchange. Дополнительные сведения см. в разделе [Управление списками адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Пользователь может быть показан в списке адресов в Azure Active Directory. Дополнительные сведения см. в разделе [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 