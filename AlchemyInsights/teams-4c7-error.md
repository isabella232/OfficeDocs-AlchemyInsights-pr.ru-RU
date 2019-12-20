---
title: Ошибка 4c7 Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796328"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="6f3b1-102">Ошибка 4c7 в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6f3b1-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="6f3b1-103">Эта ошибка возникает, потому что для Microsoft Teams требуется проверка подлинности на формах.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="6f3b1-104">При развертывании служб федерации Active Directory (AD FS) проверка подлинности по умолчанию для интрасети по умолчанию отключена.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="6f3b1-105">Если произойдет сбой встроенной проверки подлинности Windows, вам будет предложено выполнить вход с использованием проверки подлинности на основе форм.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="6f3b1-106">Чтобы устранить эту проблему, включите проверку подлинности на основе форм с помощью оснастки консоли управления (MMC) AD FS на компьютере с локальной копией Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="6f3b1-107">Для этого выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6f3b1-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="6f3b1-108">В области навигации перейдите к **политикам проверки подлинности**.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="6f3b1-109">В разделе **действия** в области сведений выберите **изменить глобальную основную проверку подлинности**.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="6f3b1-110">На вкладке **интрасеть** выберите **Проверка подлинности с помощью форм**.</span><span class="sxs-lookup"><span data-stu-id="6f3b1-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="6f3b1-111">Нажмите кнопку **ОК** (или **Применить**).</span><span class="sxs-lookup"><span data-stu-id="6f3b1-111">Select **OK** (or **Apply**).</span></span>