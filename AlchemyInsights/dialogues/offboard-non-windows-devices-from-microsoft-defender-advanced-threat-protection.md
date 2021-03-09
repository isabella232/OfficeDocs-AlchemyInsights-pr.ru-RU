---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530217"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="f7024-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="f7024-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="f7024-103">Вот как это сделать:</span><span class="sxs-lookup"><span data-stu-id="f7024-103">Here's how:</span></span>

1. <span data-ttu-id="f7024-104">Следуйте документации сторонних сторон для отключения сторонних решений от ATP Защитника Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f7024-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="f7024-105">В клиенте Azure Active Directory удалите разрешения на стороннее решение:</span><span class="sxs-lookup"><span data-stu-id="f7024-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="f7024-106">Войдите на [портал Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="f7024-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="f7024-107">Выберите **все службы**  >  **Azure Active Directory**  >  **Корпоративные приложения.**</span><span class="sxs-lookup"><span data-stu-id="f7024-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="f7024-108">Выберите приложение, которое вы хотите отключить.</span><span class="sxs-lookup"><span data-stu-id="f7024-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="f7024-109">Выберите **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="f7024-109">Select **Delete**.</span></span>

<span data-ttu-id="f7024-110">Подробнее см. в таблице [Offboard non-Windows devices.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="f7024-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
