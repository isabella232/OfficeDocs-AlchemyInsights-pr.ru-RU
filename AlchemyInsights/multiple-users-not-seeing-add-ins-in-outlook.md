---
title: Многие пользователи не видят надстройки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154583"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Многие пользователи не видят надстройки в Outlook

Если вы тестируете надстройки Outlook и они не отображаются, в качестве первого действия по устранению неполадок используйте командлет PowerShell **Get-OrganizationConfig**, чтобы запросить параметр _AppsForOfficeEnabled_. Если запрос возвращает значение **False**, настройте для этого параметра значение **True** с помощью командлета **Set-OrganizationConfig**, чтобы надстройки отображались должным образом.

Не рекомендуется устанавливать для параметра _AppsForOfficeEnabled_ значение **False**. Значение **False** переопределяет все указанные выше параметры административных и пользовательских ролей и блокирует активацию всех новых приложений любым пользователем в организации.

Дополнительные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).