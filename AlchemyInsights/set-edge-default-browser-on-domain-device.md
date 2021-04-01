---
title: Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве, присоединенном к домену
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426894"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="9f7de-102">Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве, присоединенном к домену</span><span class="sxs-lookup"><span data-stu-id="9f7de-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="9f7de-103">Настройка Microsoft Edge в качестве браузера по умолчанию</span><span class="sxs-lookup"><span data-stu-id="9f7de-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="9f7de-104">[Создайте файл конфигурации связей по умолчанию](https://go.microsoft.com/fwlink/?linkid=2132437) и сохраните его локально или в сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="9f7de-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="9f7de-105">Откройте редактор групповой политики и перейдите в **Конфигурация компьютера** > **Административные шаблоны** > **Компоненты Windows** > **Проводник**.</span><span class="sxs-lookup"><span data-stu-id="9f7de-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="9f7de-106">Выберите **Установить файл связей по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="9f7de-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="9f7de-107">Выберите **Установка параметров конфиденциальности** и нажмите **Вкл.**.</span><span class="sxs-lookup"><span data-stu-id="9f7de-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="9f7de-108">В разделе **Параметры** введите расположение файла конфигурации связей по умолчанию, а затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9f7de-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
