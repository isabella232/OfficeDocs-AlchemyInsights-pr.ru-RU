---
title: Устранение ошибки 0x8004de40 в OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525072"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="5de74-102">Устранение ошибки 0x8004de40 в OneDrive</span><span class="sxs-lookup"><span data-stu-id="5de74-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="5de74-103">Если вы получили сообщение об ошибке 0x8004de40 в OneDrive:</span><span class="sxs-lookup"><span data-stu-id="5de74-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="5de74-104">Перезагрузите компьютер, подключенный к домену АЦитве.</span><span class="sxs-lookup"><span data-stu-id="5de74-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="5de74-105">Если перезагрузка не решает проблему, отсоедините устройство от Azure AD и снова присоедините к нему.</span><span class="sxs-lookup"><span data-stu-id="5de74-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="5de74-106">**Примечание**. при выполнении этих действий вы должны находиться в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="5de74-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="5de74-107">Не выполняйте эти действия, если вы не можете подключаться к корпоративной инфраструктуре (например, в поездках).</span><span class="sxs-lookup"><span data-stu-id="5de74-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="5de74-108">Откройте окно командной строки с повышенными полномочиями.</span><span class="sxs-lookup"><span data-stu-id="5de74-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="5de74-109">Чтобы открыть командную строку с повышенными привилегиями, нажмите кнопку **Пуск**, щелкните правой кнопкой мыши **Командная строка**и выберите пункт **Запуск от имени администратора**.</span><span class="sxs-lookup"><span data-stu-id="5de74-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="5de74-110">Введите *дсрегкмд/леаве* и нажмите клавишу **Ввод**.</span><span class="sxs-lookup"><span data-stu-id="5de74-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="5de74-111">По завершении введите *дсрегкмд/Жоин* и нажмите клавишу **Ввод**.</span><span class="sxs-lookup"><span data-stu-id="5de74-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="5de74-112">По завершении закройте командную строку.</span><span class="sxs-lookup"><span data-stu-id="5de74-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="5de74-113">Перезагрузите компьютер и войдите в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5de74-113">Reboot the computer, and log into OneDrive.</span></span>