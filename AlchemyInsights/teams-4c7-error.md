---
title: Ошибка 4c7 Teams
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700216"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="c1585-102">Ошибка 4c7 в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c1585-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="c1585-103">Эта ошибка возникает, потому что для Microsoft Teams требуется проверка подлинности на формах.</span><span class="sxs-lookup"><span data-stu-id="c1585-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="c1585-104">При развертывании служб федерации Active Directory (AD FS) проверка подлинности по умолчанию для интрасети по умолчанию отключена.</span><span class="sxs-lookup"><span data-stu-id="c1585-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="c1585-105">Если произойдет сбой встроенной проверки подлинности Windows, вам будет предложено выполнить вход с использованием проверки подлинности на основе форм.</span><span class="sxs-lookup"><span data-stu-id="c1585-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="c1585-106">Чтобы устранить эту проблему, включите проверку подлинности на основе форм с помощью оснастки консоли управления (MMC) AD FS на компьютере с локальной копией Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1585-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="c1585-107">Для этого выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c1585-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="c1585-108">В области навигации перейдите к **политикам проверки подлинности**.</span><span class="sxs-lookup"><span data-stu-id="c1585-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="c1585-109">В разделе **действия** в области сведений выберите **изменить глобальную основную проверку подлинности**.</span><span class="sxs-lookup"><span data-stu-id="c1585-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="c1585-110">На вкладке **интрасеть** выберите **Проверка подлинности с помощью форм**.</span><span class="sxs-lookup"><span data-stu-id="c1585-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="c1585-111">Нажмите кнопку **ОК** (или **Применить**).</span><span class="sxs-lookup"><span data-stu-id="c1585-111">Select **OK** (or **Apply**).</span></span>