---
title: Невозможно установить или просмотреть политику AllowSelfServicePurchase
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
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826104"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9aba4-102">Невозможно установить или просмотреть политику AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="9aba4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9aba4-103">При попытке настроить или просмотреть политику AllowSelfServicePurchase вы получите следующее сообщение об ошибке:</span><span class="sxs-lookup"><span data-stu-id="9aba4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9aba4-104">*HandleError. Не удалось получить политику продукта с помощью PolicyId 'AllowSelfServicePurchase', ErrorMessage . При отправке было закрыто первое подключение. При отправке произошла неожиданная ошибка.*</span><span class="sxs-lookup"><span data-stu-id="9aba4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9aba4-105">Это может быть связано со старой версией безопасности транспортного слоя (TLS).</span><span class="sxs-lookup"><span data-stu-id="9aba4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9aba4-106">Чтобы подключить службу MSCommerce, необходимо использовать TLS 1.2 или более.</span><span class="sxs-lookup"><span data-stu-id="9aba4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9aba4-107">Попробуйте следующие действия, чтобы включить и установить протокол TLS до 1.2, проверить и повторить.</span><span class="sxs-lookup"><span data-stu-id="9aba4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9aba4-108">В командной подсказке PowerShell (PS C: введите следующую команду, чтобы установить протокол TLS версии \) 1.2:</span><span class="sxs-lookup"><span data-stu-id="9aba4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="9aba4-109">Убедитесь в использовании протокола TLS со следующей командой:</span><span class="sxs-lookup"><span data-stu-id="9aba4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="9aba4-110">Повторное просмотр команд Get или Update по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="9aba4-110">Retry the Get or Update commands as needed.</span></span>

