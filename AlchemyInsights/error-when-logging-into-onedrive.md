---
title: 0x8004de40 при запуске OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813665"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="381af-102">0x8004de40 при запуске OneDrive</span><span class="sxs-lookup"><span data-stu-id="381af-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="381af-103">Если при входе в OneDrive **0x8004de40** ошибка, перезагружайте компьютер, подключив его к работе или школьному домену.</span><span class="sxs-lookup"><span data-stu-id="381af-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="381af-104">Если вы получили эту ошибку после перезагрузки, попробуйте ее, подключившись к работе или школьному домену:</span><span class="sxs-lookup"><span data-stu-id="381af-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="381af-105">Нажмите кнопку Начните  и введите **командную** команду или командную подсказку в поле поиска, нажмите правой кнопкой мыши на командном запросе и выберите **Выполнить в качестве администратора.**</span><span class="sxs-lookup"><span data-stu-id="381af-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="381af-106">Если вам предложен пароль администратора или подтверждение, введите пароль или нажмите **кнопку Разрешить**.</span><span class="sxs-lookup"><span data-stu-id="381af-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="381af-107">В окне Командная подсказка введите **dsregcmd/leave**  и дождись завершения команды.</span><span class="sxs-lookup"><span data-stu-id="381af-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="381af-108">Затем **введите dsregcmd/join** и дождитесь завершения команды.</span><span class="sxs-lookup"><span data-stu-id="381af-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="381af-109">Перезагрузка компьютера.</span><span class="sxs-lookup"><span data-stu-id="381af-109">Reboot your computer.</span></span>
