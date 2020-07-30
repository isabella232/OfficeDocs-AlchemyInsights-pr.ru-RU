---
title: Удаление данных и очистка устройств в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434634"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="7879e-102">Удаление данных и очистка устройств в Intune</span><span class="sxs-lookup"><span data-stu-id="7879e-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="7879e-103">С помощью удаленных действий снятия с учета и очистки устройств можно удалить данные компании, находящиеся под управлением Intune, или выполнить сброс параметров устройства и восстановить параметры по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7879e-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="7879e-104">Войдите на панель мониторинга "Управление устройствами Microsoft 365", перейдите в раздел **Устройства** > **Все устройства**.</span><span class="sxs-lookup"><span data-stu-id="7879e-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="7879e-105">Выберите устройство, которое нужно очистить.</span><span class="sxs-lookup"><span data-stu-id="7879e-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="7879e-106">Выберите тип удаленной очистки.</span><span class="sxs-lookup"><span data-stu-id="7879e-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="7879e-107">При снятии с учета удаляются только данные организации. При полной очистке восстанавливаются заводские параметры устройства.</span><span class="sxs-lookup"><span data-stu-id="7879e-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="7879e-108">Нажмите кнопку **Да** для подтверждения.</span><span class="sxs-lookup"><span data-stu-id="7879e-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="7879e-109">До завершения очистки для устройства отображается состояние действия "Снятие с учета ожидается".</span><span class="sxs-lookup"><span data-stu-id="7879e-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="7879e-110">После завершения этого действия это мобильное устройство перестанет отображаться в списке управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7879e-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="7879e-111">**Примечание.** Данные компании невозможно удалить с устройств, присоединенных к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7879e-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="7879e-112">Подробные сведения о действиях снятия с учета и очистки, включая сведения о том, какие данные сохраняются, а какие — удаляются, см. в статье [Удаление устройств с помощью очистки, снятия с учета или отмены регистрации вручную](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="7879e-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="7879e-113">Сведения об удалении всех данных с устройств macOS см. в статье [Удаление всех данных с устройства macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="7879e-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>