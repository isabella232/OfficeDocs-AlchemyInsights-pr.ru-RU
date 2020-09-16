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
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745304"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="e0aff-102">Настройка функции "Файлы по запросу"</span><span class="sxs-lookup"><span data-stu-id="e0aff-102">Configure Files On-Demand</span></span>

<span data-ttu-id="e0aff-103">Функция "Файлы из OneDrive по запросу" позволяет получать доступ к файлам в OneDrive, не скачивая их все на свое устройство.</span><span class="sxs-lookup"><span data-stu-id="e0aff-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="e0aff-104">Чтобы настроить функцию "Файлы по запросу" на своем компьютере, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="e0aff-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="e0aff-105">Щелкните белый или синий значок облака **OneDrive** в области уведомлений на панели задач Windows.</span><span class="sxs-lookup"><span data-stu-id="e0aff-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="e0aff-106">Нажмите значок шестеренки **Справка и параметры** > **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="e0aff-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="e0aff-107">На вкладке **Параметры** установите флажок **Экономить место, скачивая файлы по мере необходимости**.</span><span class="sxs-lookup"><span data-stu-id="e0aff-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="e0aff-108">Вы также можете настроить функцию "Файлы по запросу" с помощью реестра.</span><span class="sxs-lookup"><span data-stu-id="e0aff-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="e0aff-109">Если вы отключите этот параметр, процедура синхронизации для пользователей Windows 10 будет той же, что и для пользователей предыдущих версий Windows, и они не смогут включить функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="e0aff-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="e0aff-110">Если вы не настраиваете этот параметр, пользователи могут включать и отключать функцию "Файлы по запросу".</span><span class="sxs-lookup"><span data-stu-id="e0aff-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="e0aff-111">Включение этой политики устанавливает значение 1 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="e0aff-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="e0aff-112">Выключение этой политики устанавливает значение 0 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="e0aff-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="e0aff-113">Если вы не видите параметра "Файлы по запросу" в разделе "Параметры", убедитесь в том, что тип запуска "Windows Cloud Files Filter Driver" имеет значение 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="e0aff-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="e0aff-114">При включении этой функции устанавливается значение 2 для следующего раздела реестра:</span><span class="sxs-lookup"><span data-stu-id="e0aff-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`