---
title: Удаление данных и очистка устройств в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416326"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="fd365-102">Удаление данных и очистка устройств в Intune</span><span class="sxs-lookup"><span data-stu-id="fd365-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="fd365-103">С помощью удаленных действий снятия с учета и очистки устройств можно удалить данные компании, находящиеся под управлением Intune, или выполнить сброс параметров устройства и восстановить параметры по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fd365-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="fd365-104">Войдите на панель мониторинга "Управление устройствами Microsoft 365", перейдите в раздел **Устройства** > **Все устройства**.</span><span class="sxs-lookup"><span data-stu-id="fd365-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="fd365-105">Выберите устройство, которое нужно очистить.</span><span class="sxs-lookup"><span data-stu-id="fd365-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="fd365-106">Выберите тип удаленной очистки.</span><span class="sxs-lookup"><span data-stu-id="fd365-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="fd365-107">При снятии с учета удаляются только данные организации. При полной очистке восстанавливаются заводские параметры устройства.</span><span class="sxs-lookup"><span data-stu-id="fd365-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="fd365-108">Нажмите кнопку **Да** для подтверждения.</span><span class="sxs-lookup"><span data-stu-id="fd365-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="fd365-109">До завершения очистки для устройства отображается состояние действия *Снятие с учета ожидается*.</span><span class="sxs-lookup"><span data-stu-id="fd365-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="fd365-110">После завершения этого действия это мобильное устройство перестанет отображаться в списке управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="fd365-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="fd365-111">Данные компании невозможно удалить с устройств, ПРИСОЕДИНЕННЫХ к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd365-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="fd365-112">Подробные сведения о действиях снятия с учета и очистки, включая сведения о том, какие данные сохраняются, а какие — удаляются, см. в документации ниже:</span><span class="sxs-lookup"><span data-stu-id="fd365-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="fd365-113">[Удаление устройств с помощью очистки, снятия с учета или отмены регистрации вручную](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="fd365-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- <span data-ttu-id="fd365-114">[Порядок очистки только корпоративных данных из приложений под управлением Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe).</span><span class="sxs-lookup"><span data-stu-id="fd365-114">[How to wipe only corporate data from Intune-managed apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)</span></span>
- <span data-ttu-id="fd365-115">[Удаление всех данных с устройства macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="fd365-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>