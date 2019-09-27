---
title: Расположение данных
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207274"
---
# <a name="data-location"></a><span data-ttu-id="594c1-102">Расположение данных</span><span class="sxs-lookup"><span data-stu-id="594c1-102">Data location</span></span>

<span data-ttu-id="594c1-103">Вы можете просмотреть расположение клиента Office 365 в центре администрирования или подключиться к Exchange Online с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="594c1-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="594c1-104">**Центр администрирования:**</span><span class="sxs-lookup"><span data-stu-id="594c1-104">**Admin center:**</span></span>
1. <span data-ttu-id="594c1-105">Выполните вход в [центр администрирования](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="594c1-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="594c1-106">Выберите **параметр** > **профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="594c1-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="594c1-107">В разделе **расположение данных**выберите **Просмотреть сведения**.</span><span class="sxs-lookup"><span data-stu-id="594c1-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="594c1-108">**Типов**</span><span class="sxs-lookup"><span data-stu-id="594c1-108">**PowerShell:**</span></span>
1. <span data-ttu-id="594c1-109">Подключитесь к Exchange Online с помощью Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="594c1-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="594c1-110">Выполните командлет [Get – OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) для отображения списка свойств клиента.</span><span class="sxs-lookup"><span data-stu-id="594c1-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="594c1-111">Просмотрите свойство Организатионид.</span><span class="sxs-lookup"><span data-stu-id="594c1-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="594c1-112">Если у вас есть расположение данных для EXO и SPO, вы можете определить расположение данных для других служб, из которых можно использовать [данные](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="594c1-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>