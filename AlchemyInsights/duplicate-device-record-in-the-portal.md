---
title: Дублирующаяся запись об устройстве на портале
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678517"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="bdc4a-102">Дублирующаяся запись об устройстве на портале</span><span class="sxs-lookup"><span data-stu-id="bdc4a-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="bdc4a-103">Если устройство не сообщает корректно о состоянии совместного управления сайту Configuration Manager, то на портале можно увидеть 2 записи для устройства.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="bdc4a-104">Чтобы проверить состояние совместного управления устройства, просмотрите столбец **Совместное управление** для устройства в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="bdc4a-105">Если столбец не отображается, то его можно добавить, щелкнув правой кнопкой мыши на любом из заголовков столбцов и выбрав его из списка.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="bdc4a-106">Значение для совместного управления должно быть **Да**.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="bdc4a-107">Если значение **Нет**, откройте клиентский компонент Configuration Manager на клиентском устройстве и установите флажок **Совместное управление** на вкладке "Общие".</span><span class="sxs-lookup"><span data-stu-id="bdc4a-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="bdc4a-108">Если значение имеет статус **Включено**, то это означает проблемы подключения клиента к точке управления.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="bdc4a-109">Дополнительные сведения о возможных неполадках подключения см. в **CcmMessaging.log** на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="bdc4a-110">Если значение имеет статус **Отключено** и устройство зарегистрировано в Intune, то убедитесь, что устройство получило Политику совместного управления, просмотрев **CoManagementHandler.log** на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bdc4a-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
