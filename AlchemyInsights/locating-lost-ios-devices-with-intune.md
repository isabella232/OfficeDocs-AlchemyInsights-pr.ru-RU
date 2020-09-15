---
title: Обнаружение потерянных устройств с iOS в Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675187"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="af149-102">Обнаружение потерянных устройств с iOS в Intune</span><span class="sxs-lookup"><span data-stu-id="af149-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="af149-103">Если включить режим пропажи на устройстве с iOS, администратор сможет получать сообщения и контактные номера телефонов, отображаемые на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="af149-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="af149-104">После включения режима пропажи администратор может использовать функцию "Поиск устройства" для определения физического расположения устройства.</span><span class="sxs-lookup"><span data-stu-id="af149-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="af149-105">Функцию "Поиск устройства" в Intune можно использовать на устройствах с iOS, чтобы показать расположение определенного устройства на карте.</span><span class="sxs-lookup"><span data-stu-id="af149-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="af149-106">Для использования этого действия необходимо, чтобы устройство iOS было в:</span><span class="sxs-lookup"><span data-stu-id="af149-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="af149-107">защищенном режиме;</span><span class="sxs-lookup"><span data-stu-id="af149-107">Supervised mode</span></span>
- <span data-ttu-id="af149-108">режиме пропажи.</span><span class="sxs-lookup"><span data-stu-id="af149-108">Lost mode</span></span>

<span data-ttu-id="af149-109">Дополнительные сведения см. в статье [Включить режим пропажи на устройствах с iOS и iPadOS с Intune](https://docs.microsoft.com/intune/device-lost-mode) и [Поиск потерянных или украденных устройств с iOS и iPadOS с Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="af149-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="af149-110">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="af149-110">**FAQ**</span></span>

<span data-ttu-id="af149-111">Вопрос. Я запустил удаленное действие для удаления данных компании с устройства, но оно зависло в состоянии ожидания.</span><span class="sxs-lookup"><span data-stu-id="af149-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="af149-112">Ответ. Для успешного выполнения удаленного действия целевое устройство должно быть подключено к сети и исправно.</span><span class="sxs-lookup"><span data-stu-id="af149-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="af149-113">В следующих ситуациях удаленное действие сохраняется в состоянии ожидания на 30 дней или до подтверждения команды на устройстве:</span><span class="sxs-lookup"><span data-stu-id="af149-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="af149-114">При отсутствии подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="af149-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="af149-115">При утрате состояния управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="af149-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="af149-116">Если вы считаете, что устройство больше не регистрируется и не сможет удалить данные компании, выберите "Удалить".</span><span class="sxs-lookup"><span data-stu-id="af149-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="af149-117">При удалении удаляется запись устройства, поэтому оно больше не отображается в списке устройств Intune.</span><span class="sxs-lookup"><span data-stu-id="af149-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="af149-118">Если устройство снова будет активным, то потребуется заново его зарегистрировать.</span><span class="sxs-lookup"><span data-stu-id="af149-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="af149-119">Вопрос. Почему некоторые удаленные действия недоступны для использования?</span><span class="sxs-lookup"><span data-stu-id="af149-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="af149-120">Ответ. Не все платформы поддерживают все удаленные действия с устройствами.</span><span class="sxs-lookup"><span data-stu-id="af149-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="af149-121">Указанные ниже удаленные действия можно использовать только для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="af149-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="af149-122">Обход блокировки активации (только iOS)</span><span class="sxs-lookup"><span data-stu-id="af149-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="af149-123">Начать заново (только Windows)</span><span class="sxs-lookup"><span data-stu-id="af149-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="af149-124">Режим утери (только iOS)</span><span class="sxs-lookup"><span data-stu-id="af149-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="af149-125">Обнаружить устройство (только iOS)</span><span class="sxs-lookup"><span data-stu-id="af149-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="af149-126">Перезапуск (только Windows)</span><span class="sxs-lookup"><span data-stu-id="af149-126">Restart (Windows only)</span></span>

<span data-ttu-id="af149-127">Дополнительные сведения о каждом из этих действий см. в статье [Доступные действия устройств](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="af149-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>