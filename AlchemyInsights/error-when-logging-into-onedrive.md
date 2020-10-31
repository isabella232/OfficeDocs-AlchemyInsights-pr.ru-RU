---
title: Ошибка 0x8004de40 при запуске OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816023"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b5399-102">Ошибка 0x8004de40 при запуске OneDrive</span><span class="sxs-lookup"><span data-stu-id="b5399-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b5399-103">При получении сообщения об ошибке **0x8004de40** при входе в OneDrive перезагрузите компьютер, подключенный к рабочему или учебному домену.</span><span class="sxs-lookup"><span data-stu-id="b5399-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b5399-104">Если после перезагрузки возникает эта ошибка, попробуйте подключиться к рабочему или учебному домену:</span><span class="sxs-lookup"><span data-stu-id="b5399-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b5399-105">Нажмите кнопку Пуск и введите в поле поиска **cmd** или **командную строку**  , щелкните правой кнопкой мыши приложение командной строки и выберите  **Запуск от имени администратора** .</span><span class="sxs-lookup"><span data-stu-id="b5399-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="b5399-106">При получении запроса на ввод пароля администратора или подтверждения введите пароль или нажмите кнопку **Разрешить** .</span><span class="sxs-lookup"><span data-stu-id="b5399-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="b5399-107">В окне командной строки введите **дсрегкмд/леаве**  и дождитесь завершения команды.</span><span class="sxs-lookup"><span data-stu-id="b5399-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b5399-108">Затем введите **дсрегкмд/Жоин** и дождитесь завершения команды.</span><span class="sxs-lookup"><span data-stu-id="b5399-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b5399-109">Перезагрузите компьютер.</span><span class="sxs-lookup"><span data-stu-id="b5399-109">Reboot your computer.</span></span>
