---
title: PowerShell в SharePoint Online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764274"
---
# <a name="sharepoint-online-powershell"></a>PowerShell в SharePoint Online

Работаете с PowerShell или сценариями в SharePoint Online? Для получения дополнительных сведений посетите приведенные ниже ссылки.
- [Начало работы с командной консолью SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Подключение к SPO PowerShell с многофакторной проверкой подлинности (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Шаблоны и методики SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) содержат библиотеку команд PowerShell, которая позволяет выполнять сложные действия по управлению для SPO.

> [!NOTE]
> - Если у вас возникли проблемы с подключением к командной консоли SPO, убедитесь, что вы обновили последнюю версию и пытаетесь [повторно импортировать модуль](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) с помощью командлета *"Import-Module Microsoft. Online. SharePoint. PowerShell".*
> - При попытке запустить скрипты объектной модели на стороне клиента на локальном компьютере должен быть установлен [пакет SDK для клиентских компонентов SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .
> - Если у вас возникли проблемы с запуском сценариев из PowerShell, вы можете использовать PowerShell от имени администратора и изменить [политику выполнения](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).