---
title: Самостоятельная Покупка PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091753"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="9d9b9-102">Самостоятельная Покупка PowerShell</span><span class="sxs-lookup"><span data-stu-id="9d9b9-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="9d9b9-103">Чтобы использовать модуль PowerShell Мскоммерце, его необходимо установить на устройстве с Windows 10 с TLS 1,2 (требуются разрешения локального администратора).</span><span class="sxs-lookup"><span data-stu-id="9d9b9-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="9d9b9-104">Импортируйте модуль Мскоммерце и подключитесь к нему.</span><span class="sxs-lookup"><span data-stu-id="9d9b9-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="9d9b9-105">При получении запроса на вход в систему необходимо использовать учетные данные роли администратора глобальной или выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="9d9b9-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="9d9b9-106">Если у вас нет протокола TLS 1,2, при попытке получить или изменить политику вы можете получить следующее сообщение об ошибке:</span><span class="sxs-lookup"><span data-stu-id="9d9b9-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="9d9b9-107">*ErrorMessage — базовое подключение было закрыто: при отправке произошла непредвиденная ошибка*.</span><span class="sxs-lookup"><span data-stu-id="9d9b9-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



