---
title: Что делать, если функции Azure не работают должным образом в Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576598"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="f7be3-102">Что делать, если функции Azure не работают должным образом в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f7be3-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="f7be3-103">Microsoft Edge имеет [Известные проблемы](https://go.microsoft.com/fwlink/?linkid=2140608) , связанные с зонами безопасности, и может повлиять на то, как пользователи Azure входят в центр администрирования Windows.</span><span class="sxs-lookup"><span data-stu-id="f7be3-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="f7be3-104">Если у вас возникли проблемы с использованием функций Azure с Microsoft EDGE, попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="f7be3-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="f7be3-105">В меню **Пуск** выберите пункт **Свойства браузера** и выберите его.</span><span class="sxs-lookup"><span data-stu-id="f7be3-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="f7be3-106">В диалоговом окне **Свойства обозревателя** перейдите на вкладку **Безопасность** .</span><span class="sxs-lookup"><span data-stu-id="f7be3-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="f7be3-107">Выберите зону **Надежные сайты** , а затем нажмите кнопку **сайты** .</span><span class="sxs-lookup"><span data-stu-id="f7be3-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="f7be3-108">В диалоговом окне **Надежные сайты** добавьте URL-адрес шлюза, а также [https://login.microsoftonline.com](https://login.microsoftonline.com) и нажмите [https://login.live.com](https://login.live.com) кнопку **Закрыть**.</span><span class="sxs-lookup"><span data-stu-id="f7be3-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="f7be3-109">В диалоговом окне **Свойства обозревателя** перейдите на вкладку **Конфиденциальность** .</span><span class="sxs-lookup"><span data-stu-id="f7be3-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="f7be3-110">В разделе **блокирование всплывающих окон** выберите **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="f7be3-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="f7be3-111">В открывшемся диалоговом окне Добавьте URL-адрес шлюза, а также [https://login.microsoftonline.com](https://login.microsoftonline.com) и нажмите [https://login.live.com](https://login.live.com) кнопку **Закрыть**.</span><span class="sxs-lookup"><span data-stu-id="f7be3-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
