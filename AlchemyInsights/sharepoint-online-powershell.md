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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="f63da-102">PowerShell в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f63da-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="f63da-103">Работаете с PowerShell или сценариями в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="f63da-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="f63da-104">Для получения дополнительных сведений посетите приведенные ниже ссылки.</span><span class="sxs-lookup"><span data-stu-id="f63da-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="f63da-105">Начало работы с командной консолью SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f63da-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="f63da-106">Подключение к SPO PowerShell с многофакторной проверкой подлинности (MFA)</span><span class="sxs-lookup"><span data-stu-id="f63da-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="f63da-107">[Шаблоны и методики SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) содержат библиотеку команд PowerShell, которая позволяет выполнять сложные действия по управлению для SPO.</span><span class="sxs-lookup"><span data-stu-id="f63da-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="f63da-108">Если у вас возникли проблемы с подключением к командной консоли SPO, убедитесь, что вы обновили последнюю версию и пытаетесь [повторно импортировать модуль](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) с помощью командлета *"Import-Module Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="f63da-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="f63da-109">При попытке запустить скрипты объектной модели на стороне клиента на локальном компьютере должен быть установлен [пакет SDK для клиентских компонентов SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="f63da-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="f63da-110">Если у вас возникли проблемы с запуском сценариев из PowerShell, вы можете использовать PowerShell от имени администратора и изменить [политику выполнения](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="f63da-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>