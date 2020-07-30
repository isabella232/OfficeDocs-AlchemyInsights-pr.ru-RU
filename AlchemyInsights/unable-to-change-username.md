---
title: Не удалось изменить имя пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431742"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="19228-102">Не удалось изменить имя пользователя</span><span class="sxs-lookup"><span data-stu-id="19228-102">Unable to change UserName</span></span>

<span data-ttu-id="19228-103">В некоторых случаях изменения UPN (UserPrincipalName) не распространяются на облако.</span><span class="sxs-lookup"><span data-stu-id="19228-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="19228-104">Вы можете столкнуться с ошибками проверки на портале Office 365 или с невозможностью изменить имя пользователя или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="19228-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="19228-105">Чтобы устранить эту проблему, вручную настройте UserPrincipalName с помощью этой команды PowerShell.</span><span class="sxs-lookup"><span data-stu-id="19228-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="19228-106">**Пример: переименование пользователя**</span><span class="sxs-lookup"><span data-stu-id="19228-106">**Example: Rename a user**</span></span>

<span data-ttu-id="19228-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="19228-107">PowerShellCopy</span></span>

<span data-ttu-id="19228-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="19228-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="19228-109">Эта команда переименовывает davidc@contoso.com в davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="19228-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="19228-110">Дополнительные сведения см. в статье [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="19228-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>