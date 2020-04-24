---
title: Дублирующаяся запись об устройстве на портале
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790170"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="1be28-102">Дублирующаяся запись об устройстве на портале</span><span class="sxs-lookup"><span data-stu-id="1be28-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="1be28-103">Если устройство не сообщает корректно о состоянии совместного управления сайту Configuration Manager, то на портале можно увидеть 2 записи для устройства.</span><span class="sxs-lookup"><span data-stu-id="1be28-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="1be28-104">Чтобы проверить состояние совместного управления устройства, просмотрите столбец **Совместное управление** для устройства в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="1be28-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="1be28-105">Если столбец не отображается, то его можно добавить, щелкнув правой кнопкой мыши на любом из заголовков столбцов и выбрав его из списка.</span><span class="sxs-lookup"><span data-stu-id="1be28-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="1be28-106">Значение для совместного управления должно быть **Да**.</span><span class="sxs-lookup"><span data-stu-id="1be28-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="1be28-107">Если значение **Нет**, откройте клиентский компонент Configuration Manager на клиентском устройстве и установите флажок **Совместное управление** на вкладке "Общие".</span><span class="sxs-lookup"><span data-stu-id="1be28-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="1be28-108">Если значение имеет статус **Включено**, то это означает проблемы подключения клиента к точке управления.</span><span class="sxs-lookup"><span data-stu-id="1be28-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="1be28-109">Дополнительные сведения о возможных неполадках подключения см. в **CcmMessaging.log** на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1be28-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="1be28-110">Если значение имеет статус **Отключено** и устройство зарегистрировано в Intune, то убедитесь, что устройство получило Политику совместного управления, просмотрев **CoManagementHandler.log** на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1be28-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
