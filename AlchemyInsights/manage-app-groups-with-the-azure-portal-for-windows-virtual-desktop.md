---
title: Управление группами приложений с помощью портала Azure для виртуального рабочего стола Windows
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
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715721"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="4644c-102">Управление группами приложений с помощью портала Azure для виртуального рабочего стола Windows</span><span class="sxs-lookup"><span data-stu-id="4644c-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="4644c-103">Группа приложений по умолчанию, созданная для нового пула хост-приложений виртуального рабочего стола Windows, также публикует полный рабочий стол.</span><span class="sxs-lookup"><span data-stu-id="4644c-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="4644c-104">Кроме того, с помощью портала Azure можно создать одну или несколько групп приложений RemoteApp для пула хост-приложений.</span><span class="sxs-lookup"><span data-stu-id="4644c-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="4644c-105">Процесс развертывания будет делать следующее:</span><span class="sxs-lookup"><span data-stu-id="4644c-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="4644c-106">Создайте группу приложений RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="4644c-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="4644c-107">Добавьте выбранные приложения в группу приложений.</span><span class="sxs-lookup"><span data-stu-id="4644c-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="4644c-108">Публикация отдельных пользователей или групп пользователей в группе приложений.</span><span class="sxs-lookup"><span data-stu-id="4644c-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="4644c-109">Зарегистрируйте группу приложений, если вы решили сделать это.</span><span class="sxs-lookup"><span data-stu-id="4644c-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="4644c-110">Создайте ссылку на шаблон Azure Resource Manager в соответствии с конфигурацией, которую можно скачать и сохранить.</span><span class="sxs-lookup"><span data-stu-id="4644c-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="4644c-111">Чтобы создать группу RemoteApp для виртуального рабочего стола Windows, следуйте инструкциям в области управления группами приложений [на портале Azure.](https://go.microsoft.com/fwlink/?linkid=2129550)</span><span class="sxs-lookup"><span data-stu-id="4644c-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
