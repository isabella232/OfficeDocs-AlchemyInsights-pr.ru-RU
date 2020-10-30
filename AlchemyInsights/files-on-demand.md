---
title: Файлы по запросу
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791307"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="5f8d1-102">Настройка функции "Файлы по запросу"</span><span class="sxs-lookup"><span data-stu-id="5f8d1-102">Configure Files On-Demand</span></span>

<span data-ttu-id="5f8d1-103">Для работы функции "Файлы из OneDrive по запросу" требуются [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (версии 1709 или более поздней) или Windows Server 2019 и OneDrive сборки 17.3.7064.1005 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="5f8d1-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="5f8d1-104">Функция "Файлы из OneDrive по запросу" позволяет получать доступ к файлам в OneDrive, не скачивая их все на свое устройство.</span><span class="sxs-lookup"><span data-stu-id="5f8d1-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="5f8d1-105">Чтобы настроить функцию "Файлы по запросу" на своем компьютере, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="5f8d1-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="5f8d1-106">Щелкните белый или синий значок облака **OneDrive** в области уведомлений на панели задач Windows.</span><span class="sxs-lookup"><span data-stu-id="5f8d1-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="5f8d1-107">Нажмите значок шестеренки **Справка и параметры** > **Параметры** .</span><span class="sxs-lookup"><span data-stu-id="5f8d1-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="5f8d1-108">На вкладке **Параметры** установите флажок **Экономить место, скачивая файлы по мере необходимости** .</span><span class="sxs-lookup"><span data-stu-id="5f8d1-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="5f8d1-109">Вы также можете настроить функцию "Файлы по запросу" с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="5f8d1-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="5f8d1-110">Если вы отключите этот параметр, процедура синхронизации для пользователей Windows 10 будет той же, что и для пользователей предыдущих версий Windows, и они не смогут включить функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="5f8d1-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="5f8d1-111">Если вы не настраиваете этот параметр, пользователи могут включать и отключать функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="5f8d1-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="5f8d1-112">Включение этой политики устанавливает значение 1 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="5f8d1-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="5f8d1-113">Выключение этой политики устанавливает значение 0 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="5f8d1-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="5f8d1-114">Если вы не видите параметра "Файлы по запросу" в разделе "Параметры", убедитесь в том, что тип запуска "Windows Cloud Files Filter Driver" имеет значение 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="5f8d1-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="5f8d1-115">При включении этой функции устанавливается значение 2 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="5f8d1-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`