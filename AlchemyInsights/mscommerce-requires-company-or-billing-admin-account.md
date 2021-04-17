---
title: Подключение к модульу MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829749"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="a177f-102">MSCommerce требует учетную запись администратора компании или биллинга</span><span class="sxs-lookup"><span data-stu-id="a177f-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="a177f-103">Модуль MSCommerce требует учетную запись с привилегиями администратора компании или биллинга.</span><span class="sxs-lookup"><span data-stu-id="a177f-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="a177f-104">Если вы получаете следующую ошибку, вам потребуется повторно подключиться к другой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a177f-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="a177f-105">*ErrorMessage — удаленный сервер возвращает ошибку: (403) Запрещено. ErrorDetails — В C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="a177f-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="a177f-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span><span class="sxs-lookup"><span data-stu-id="a177f-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="a177f-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="a177f-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="a177f-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="a177f-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="a177f-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="a177f-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="a177f-110">Если у вашей учетной записи нет привилегий администратора компании или биллинга, обратитесь к ИТ-администратору.</span><span class="sxs-lookup"><span data-stu-id="a177f-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
