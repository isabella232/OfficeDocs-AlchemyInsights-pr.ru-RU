---
title: Не удается задать или просмотреть политику Алловселфсервицепурчасе
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
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158574"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="13453-102">Не удается задать или просмотреть политику Алловселфсервицепурчасе</span><span class="sxs-lookup"><span data-stu-id="13453-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="13453-103">При попытке задать или просмотреть политику Алловселфсервицепурчасе появляется следующее сообщение об ошибке:</span><span class="sxs-lookup"><span data-stu-id="13453-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="13453-104">*HandleError: не удалось получить политику продукта с Полициид "Алловселфсервицепурчасе", ErrorMessage — базовое подключение было закрыто: при отправке произошла непредвиденная ошибка.*</span><span class="sxs-lookup"><span data-stu-id="13453-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="13453-105">Это может быть вызвано более старой версией протокола TLS.</span><span class="sxs-lookup"><span data-stu-id="13453-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="13453-106">Чтобы подключить службу Мскоммерце, необходимо использовать протокол TLS 1,2 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="13453-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="13453-107">Выполните следующие действия, чтобы включить или отключить протокол TLS равным 1,2, проверить и повторить попытку.</span><span class="sxs-lookup"><span data-stu-id="13453-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="13453-108">В командной командной консоли PowerShell (PS C:\) введите следующую команду, чтобы установить для протокола TLS версии 1,2:</span><span class="sxs-lookup"><span data-stu-id="13453-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="13453-109">Проверьте использование протоколов TLS с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="13453-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="13453-110">Повторите команды Get или Update по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="13453-110">Retry the Get or Update commands as needed.</span></span>

