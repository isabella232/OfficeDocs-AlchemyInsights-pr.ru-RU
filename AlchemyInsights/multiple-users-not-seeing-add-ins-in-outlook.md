---
title: Многие пользователи не видят надстройки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729884"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Многие пользователи не видят надстройки в Outlook

Если вы тестируете надстройки Outlook и они не отображаются, в качестве первого действия по устранению неполадок используйте командлет PowerShell **Get-OrganizationConfig**, чтобы запросить параметр _AppsForOfficeEnabled_. Если запрос возвращает значение **False**, настройте для этого параметра значение **True** с помощью командлета **Set-OrganizationConfig**, чтобы надстройки отображались должным образом.

Не рекомендуется устанавливать для параметра _AppsForOfficeEnabled_ значение **False**. Значение **False** переопределяет все указанные выше параметры административных и пользовательских ролей и блокирует активацию всех новых приложений любым пользователем в организации.

Дополнительные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).