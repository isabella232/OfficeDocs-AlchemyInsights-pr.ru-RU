---
title: Файлы по запросу
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406602"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="12bd4-102">Настройка функции "Файлы по запросу"</span><span class="sxs-lookup"><span data-stu-id="12bd4-102">Configure Files On-Demand</span></span>

<span data-ttu-id="12bd4-103">Функция "Файлы из OneDrive по запросу" позволяет получать доступ к файлам в OneDrive, не скачивая их все на свое устройство.</span><span class="sxs-lookup"><span data-stu-id="12bd4-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="12bd4-104">Чтобы настроить функцию "Файлы по запросу" на своем компьютере, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="12bd4-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="12bd4-105">Щелкните белый или синий значок облака **OneDrive** в области уведомлений на панели задач Windows.</span><span class="sxs-lookup"><span data-stu-id="12bd4-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="12bd4-106">Нажмите значок шестеренки **Справка и параметры** > **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="12bd4-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="12bd4-107">На вкладке **Параметры** установите флажок **Экономить место, скачивая файлы по мере необходимости**.</span><span class="sxs-lookup"><span data-stu-id="12bd4-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="12bd4-108">Вы также можете настроить функцию "Файлы по запросу" с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="12bd4-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="12bd4-109">Если вы отключите этот параметр, процедура синхронизации для пользователей Windows 10 будет той же, что и для пользователей предыдущих версий Windows, и они не смогут включить функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="12bd4-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="12bd4-110">Если вы не настраиваете этот параметр, пользователи могут включать и отключать функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="12bd4-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="12bd4-111">Включение этой политики устанавливает значение 1 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="12bd4-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="12bd4-112">Выключение этой политики устанавливает значение 0 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="12bd4-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="12bd4-113">Если вы не видите параметра "Файлы по запросу" в разделе "Параметры", убедитесь в том, что тип запуска "Windows Cloud Files Filter Driver" имеет значение 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="12bd4-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="12bd4-114">При включении этой функции устанавливается значение 2 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="12bd4-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`