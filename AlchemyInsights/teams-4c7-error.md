---
title: Ошибка Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786682"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="01922-102">Ошибка 4c7 в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="01922-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="01922-103">Эта ошибка возникает из-за того, что Microsoft Teams требует проверки подлинности форм.</span><span class="sxs-lookup"><span data-stu-id="01922-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="01922-104">При развертывании служб Федерации Active Directory (AD FS) проверка подлинности форм не включена для интрасети по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="01922-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="01922-105">Если сбой в интегрированной проверке подлинности Windows, вам будет предложено войти с помощью проверки подлинности форм.</span><span class="sxs-lookup"><span data-stu-id="01922-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="01922-106">Чтобы устранить эту проблему, введи проверку подлинности форм с помощью оснастки AD FS Microsoft Management Console (MMC) на компьютере с локальной копией Active Directory.</span><span class="sxs-lookup"><span data-stu-id="01922-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="01922-107">Для этого выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="01922-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="01922-108">В области навигации просмотрите политики **проверки подлинности.**</span><span class="sxs-lookup"><span data-stu-id="01922-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="01922-109">В **области Действия** в области сведений выберите Изменить **глобальную первичную проверку подлинности.**</span><span class="sxs-lookup"><span data-stu-id="01922-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="01922-110">На **вкладке Intranet** выберите **проверку подлинности форм.**</span><span class="sxs-lookup"><span data-stu-id="01922-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="01922-111">Выберите **ОК** (или **Применить).**</span><span class="sxs-lookup"><span data-stu-id="01922-111">Select **OK** (or **Apply**).</span></span>