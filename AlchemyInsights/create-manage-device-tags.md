---
title: Создание тегов или групп устройств и управление ими
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721731"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="2f694-102">Создание тегов или групп устройств и управление ими</span><span class="sxs-lookup"><span data-stu-id="2f694-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="2f694-103">Добавьте теги на устройства, чтобы создать логическую группу.</span><span class="sxs-lookup"><span data-stu-id="2f694-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="2f694-104">Теги устройств поддерживают правильное сопоставление сети, позволяя вам присоединять различные теги для захвата контекста и включения динамического создания списков в рамках инцидента.</span><span class="sxs-lookup"><span data-stu-id="2f694-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="2f694-105">Теги можно использовать в качестве фильтра в представлении списка устройств или для группировки устройств.</span><span class="sxs-lookup"><span data-stu-id="2f694-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="2f694-106">Дополнительные сведения о группировке устройств см. в статье [Создание тегов устройств и управление ими](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="2f694-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="2f694-107">Добавлять теги на устройства, можно с помощью следующего:</span><span class="sxs-lookup"><span data-stu-id="2f694-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="2f694-108">Использование портала</span><span class="sxs-lookup"><span data-stu-id="2f694-108">Using the portal</span></span>

- <span data-ttu-id="2f694-109">Настройка значения раздела реестра</span><span class="sxs-lookup"><span data-stu-id="2f694-109">Setting a registry key value</span></span>
 
<span data-ttu-id="2f694-110">**Примечание.** Между добавлением тега на устройство, и его доступностью в списке устройств, а также на странице устройства может быть задержка.</span><span class="sxs-lookup"><span data-stu-id="2f694-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="2f694-111">Чтобы добавить теги устройств с помощью API, см. [API добавления и удаления тегов устройств](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="2f694-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="2f694-112">Добавление тегов устройств и управление ими с помощью портала</span><span class="sxs-lookup"><span data-stu-id="2f694-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="2f694-113">Выберите устройство, для которого вы хотите настроить теги.</span><span class="sxs-lookup"><span data-stu-id="2f694-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="2f694-114">Можно выбрать устройство или найти его в любом из следующих представлений:</span><span class="sxs-lookup"><span data-stu-id="2f694-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="2f694-115">**Панель мониторинга операций обеспечения безопасности** Выберите имя устройства из раздела "Устройства с активными оповещениями".</span><span class="sxs-lookup"><span data-stu-id="2f694-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="2f694-116">**Очередь оповещений** – Выберите имя устройства рядом со значком устройства из очереди оповещений.</span><span class="sxs-lookup"><span data-stu-id="2f694-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="2f694-117">**Список устройств** – Выберите имя устройства из списка устройств.</span><span class="sxs-lookup"><span data-stu-id="2f694-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="2f694-118">**Поле поиска** – Выберите устройство из раскрывающегося меню и введите имя устройства.</span><span class="sxs-lookup"><span data-stu-id="2f694-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="2f694-119">Вы также можете попасть на страницу оповещений с помощью представления файлов и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="2f694-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="2f694-120">Выберите **Управление тегами** в строке действий ответа.</span><span class="sxs-lookup"><span data-stu-id="2f694-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="2f694-121">Начните ввод для поиска или создания тегов.</span><span class="sxs-lookup"><span data-stu-id="2f694-121">Type to find or create tags.</span></span>

<span data-ttu-id="2f694-122">Теги добавляются в представление устройства и отражаются в представлении списка устройств.</span><span class="sxs-lookup"><span data-stu-id="2f694-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="2f694-123">Затем можно использовать фильтр тегов, чтобы увидеть соответствующий список устройств.</span><span class="sxs-lookup"><span data-stu-id="2f694-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="2f694-124">Дополнительные сведения см. в статье [Создание тегов устройств и управление ими](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="2f694-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>