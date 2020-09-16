---
title: Самостоятельная Покупка PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739983"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="ebef6-102">Самостоятельная Покупка PowerShell</span><span class="sxs-lookup"><span data-stu-id="ebef6-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="ebef6-103">Чтобы использовать модуль PowerShell Мскоммерце, его необходимо установить на устройстве с Windows 10 с TLS 1,2 (требуются разрешения локального администратора).</span><span class="sxs-lookup"><span data-stu-id="ebef6-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="ebef6-104">Импортируйте модуль Мскоммерце и подключитесь к нему.</span><span class="sxs-lookup"><span data-stu-id="ebef6-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="ebef6-105">При получении запроса на вход в систему необходимо использовать учетные данные роли администратора глобальной или выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ebef6-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="ebef6-106">Если у вас нет протокола TLS 1,2, при попытке получить или изменить политику вы можете получить следующее сообщение об ошибке:</span><span class="sxs-lookup"><span data-stu-id="ebef6-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="ebef6-107">*ErrorMessage — базовое подключение было закрыто: при отправке произошла непредвиденная ошибка*.</span><span class="sxs-lookup"><span data-stu-id="ebef6-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



