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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Установка Office и OneDrive на Виртуальном рабочем столе Windows

1. [Подготовьте и настройте главный образ VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Создайте виртуальную машину (VM), если она еще не создана.

1. [Установите Office в режиме активации на общем компьютере](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Активация на общем компьютере позволяет нескольким пользователям получить доступ к Office.

1. [Установите OneDrive в режиме для каждого компьютера](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Как правило, OneDrive устанавливается для каждого пользователя, но в данном случае он должен быть установлен для каждого компьютера.