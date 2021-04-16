---
title: Самообслуживка покупки PowerShell
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797734"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="e3b38-102">Самообслуживка покупки PowerShell</span><span class="sxs-lookup"><span data-stu-id="e3b38-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="e3b38-103">Чтобы использовать модуль MSCommerce PowerShell, необходимо установить его на устройство Windows 10 с TLS 1.2 (необходимые разрешения локального администратора).</span><span class="sxs-lookup"><span data-stu-id="e3b38-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="e3b38-104">Импорт и подключение к модульу MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="e3b38-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="e3b38-105">Если вам будет предложено войти в систему, вам потребуется использовать учетные данные global или Billing Admin role.</span><span class="sxs-lookup"><span data-stu-id="e3b38-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="e3b38-106">Если у вас нет TLS 1.2, при попытке получить или обновить политику можно получить следующую ошибку:</span><span class="sxs-lookup"><span data-stu-id="e3b38-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="e3b38-107">*ErrorMessage — подключение* было закрыто: при отправке произошла неожиданная ошибка.</span><span class="sxs-lookup"><span data-stu-id="e3b38-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



