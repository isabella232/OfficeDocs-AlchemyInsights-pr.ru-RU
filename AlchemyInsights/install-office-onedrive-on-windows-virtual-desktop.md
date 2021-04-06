---
title: Установка Office и OneDrive на Виртуальном рабочем столе Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590291"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="e7623-102">Установка Office и OneDrive на Виртуальном рабочем столе Windows</span><span class="sxs-lookup"><span data-stu-id="e7623-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="e7623-103">[Подготовьте и настройте главный образ VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="e7623-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="e7623-104">Создайте виртуальную машину (VM), если она еще не создана.</span><span class="sxs-lookup"><span data-stu-id="e7623-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="e7623-105">[Установите Office в режиме активации на общем компьютере](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span><span class="sxs-lookup"><span data-stu-id="e7623-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="e7623-106">Активация на общем компьютере позволяет нескольким пользователям получить доступ к Office.</span><span class="sxs-lookup"><span data-stu-id="e7623-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="e7623-107">[Установите OneDrive в режиме для каждого компьютера](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span><span class="sxs-lookup"><span data-stu-id="e7623-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="e7623-108">Как правило, OneDrive устанавливается для каждого пользователя, но в данном случае он должен быть установлен для каждого компьютера.</span><span class="sxs-lookup"><span data-stu-id="e7623-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>