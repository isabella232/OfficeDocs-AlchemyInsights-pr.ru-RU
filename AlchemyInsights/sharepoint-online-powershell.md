---
title: PowerShell в SharePoint Online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123011"
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