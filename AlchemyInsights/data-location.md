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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655295"
---
# <a name="data-location"></a><span data-ttu-id="eceef-102">Расположение данных</span><span class="sxs-lookup"><span data-stu-id="eceef-102">Data location</span></span>

<span data-ttu-id="eceef-103">Вы можете просмотреть расположение клиента в центре администрирования или подключиться к Exchange Online с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="eceef-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="eceef-104">**Центр администрирования:**</span><span class="sxs-lookup"><span data-stu-id="eceef-104">**Admin center:**</span></span>
1. <span data-ttu-id="eceef-105">Выполните вход в [центр администрирования](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="eceef-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="eceef-106">Выберите **параметр** > **профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="eceef-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="eceef-107">В разделе **расположение данных**выберите **Просмотреть сведения**.</span><span class="sxs-lookup"><span data-stu-id="eceef-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="eceef-108">**Типов**</span><span class="sxs-lookup"><span data-stu-id="eceef-108">**PowerShell:**</span></span>
1. <span data-ttu-id="eceef-109">Подключитесь к Exchange Online с помощью Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="eceef-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="eceef-110">Выполните командлет [Get – OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) для отображения списка свойств клиента.</span><span class="sxs-lookup"><span data-stu-id="eceef-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="eceef-111">Просмотрите свойство Организатионид.</span><span class="sxs-lookup"><span data-stu-id="eceef-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="eceef-112">Если у вас есть расположение данных для EXO и SPO, вы можете определить расположение данных для других служб, из которых можно использовать [данные](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="eceef-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>