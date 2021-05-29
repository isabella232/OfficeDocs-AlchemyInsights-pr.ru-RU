---
title: DLP конечной точки не развернута на устройстве пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694813"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="a25b1-102">DLP конечной точки не развернута на устройстве пользователя</span><span class="sxs-lookup"><span data-stu-id="a25b1-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="a25b1-103">Если параметр защиты от потери данных (DLP) конечной точки не применен на устройстве пользователя, нужно подтвердить соответствие этим требованиям:</span><span class="sxs-lookup"><span data-stu-id="a25b1-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="a25b1-104">На устройстве установлена Windows 10 x64 сборки 1809 или более поздняя версия.</span><span class="sxs-lookup"><span data-stu-id="a25b1-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="a25b1-105">Установлен клиент для защиты от вредоносных программ версии 4.18.2009.7 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="a25b1-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="a25b1-106">Устройство является **одним** из следующих:</span><span class="sxs-lookup"><span data-stu-id="a25b1-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="a25b1-107">С присоединением к Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="a25b1-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="a25b1-108">С гибридным присоединением к Azure AD</span><span class="sxs-lookup"><span data-stu-id="a25b1-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="a25b1-109">С регистрацией в AAD</span><span class="sxs-lookup"><span data-stu-id="a25b1-109">AAD registered</span></span>

- <span data-ttu-id="a25b1-110">Чтобы применить действие политики, убедитесь в том, что браузер Microsoft Chromium Edge установлен на устройстве с конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="a25b1-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="a25b1-111">Дополнительные требования к развертыванию защиты от потери данных в конечной точке см. в разделе[. Начало работы с функцией защиты от потери данных](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="a25b1-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>