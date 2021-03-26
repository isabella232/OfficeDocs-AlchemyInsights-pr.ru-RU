---
title: Справка по настройке ночного света для дисплея
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123143"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="82988-102">Справка по настройке ночного света для дисплея</span><span class="sxs-lookup"><span data-stu-id="82988-102">Help with the night light display setting</span></span>

<span data-ttu-id="82988-103">Дополнительные сведения о настройке ночного света для дисплея см. в разделе [Настройка ночного света для дисплея в Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="82988-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="82988-104">Если параметры ночного света в настройках неактивны, проверьте драйвер дисплея.</span><span class="sxs-lookup"><span data-stu-id="82988-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="82988-105">В поле поиска на панели задач введите **Диспетчер устройств**, а затем выберите **Диспетчер устройств** в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="82988-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="82988-106">Разверните **Адаптеры дисплея**.</span><span class="sxs-lookup"><span data-stu-id="82988-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="82988-107">К сожалению, функция ночного света будет недоступна, если ваше устройство использует драйвер DisplayLink или базовый драйвер дисплея.</span><span class="sxs-lookup"><span data-stu-id="82988-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="82988-108">Функция ночного света использует новейшие графические технологии, поэтому вам может потребоваться обновить драйвер дисплея.</span><span class="sxs-lookup"><span data-stu-id="82988-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="82988-109">Проверьте наличие обновлений, перейдя в раздел **Пуск** > **Параметры** > **Обновление и безопасность** > **Центр обновления Windows** > **Проверить наличие обновлений**.</span><span class="sxs-lookup"><span data-stu-id="82988-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="82988-110">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="82988-110">OR</span></span>

- <span data-ttu-id="82988-111">Посетите веб-сайт службы поддержки производителя оборудования, чтобы вручную скачать и установить последние драйверы дисплея.</span><span class="sxs-lookup"><span data-stu-id="82988-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="82988-112">Сброс ночного света в реестре</span><span class="sxs-lookup"><span data-stu-id="82988-112">Reset night light in the registry</span></span>

<span data-ttu-id="82988-113">Если обновление драйвера дисплея не помогло решить проблему, возможно, вам потребуется сбросить ночной свет в реестре.</span><span class="sxs-lookup"><span data-stu-id="82988-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="82988-114">**Внимание!** Этот способ устранения неполадок рекомендуется только для опытных пользователей.</span><span class="sxs-lookup"><span data-stu-id="82988-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="82988-115">Внесение неправильных изменений в реестр может привести к возникновению серьезных проблем.</span><span class="sxs-lookup"><span data-stu-id="82988-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="82988-116">Для дополнительной защиты сделайте резервную копию реестра, прежде чем вносить в него изменения, чтобы вы могли восстановить его в случае возникновения проблем.</span><span class="sxs-lookup"><span data-stu-id="82988-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="82988-117">В поле поиска введите **regedit**, а затем выберите **Редактор реестра** в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="82988-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="82988-118">Откройте следующий раздел реестра:</span><span class="sxs-lookup"><span data-stu-id="82988-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="82988-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="82988-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="82988-120">Экспортируйте и затем удалите следующий подраздел:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="82988-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="82988-121">Экспортируйте и затем удалите следующий подраздел:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="82988-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="82988-122">Перезапустите Windows и проверьте, доступны ли параметры ночного света.</span><span class="sxs-lookup"><span data-stu-id="82988-122">Restart Windows and verify if the night light options are available.</span></span>


