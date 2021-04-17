---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830595"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Работа с PowerShell или скриптами в Sharepoint Online? Дополнительные сведения см. в ссылках ниже.
- [Начало работы с командной консолью SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Подключение к SPO PowerShell с многофакторной проверкой подлинности (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Шаблоны и практики [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) содержат библиотеку команд PowerShell, которая позволяет выполнять сложные действия по управлению SPO.

> [!NOTE]
> - Если возникли проблемы с подключением к оболочке управления SPO, убедитесь, что вы [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) обновили последнюю версию, и попробуйте повторно импортировать модуль с помощью *"Импорт-модуль Microsoft.Online.SharePoint.PowerShell".*
> - При попытке запуска сценариев клиентской объектной модели необходимо установить [SDK](https://www.microsoft.com/download/details.aspx?id=42038) клиентских компонентов Sharepoint Online на локальной машине.
> - Если у вас возникли проблемы с выполнением скриптов из PowerShell, возможно, следует рассмотреть возможность запуска PowerShell в качестве администратора и изменения [политики выполнения.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)