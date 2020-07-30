---
title: Обнаружение потерянных устройств с iOS в Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434625"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="48937-102">Обнаружение потерянных устройств с iOS в Intune</span><span class="sxs-lookup"><span data-stu-id="48937-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="48937-103">Если включить режим пропажи на устройстве с iOS, администратор сможет получать сообщения и контактные номера телефонов, отображаемые на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="48937-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="48937-104">После включения режима пропажи администратор может использовать функцию "Поиск устройства" для определения физического расположения устройства.</span><span class="sxs-lookup"><span data-stu-id="48937-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="48937-105">Функцию "Поиск устройства" в Intune можно использовать на устройствах с iOS, чтобы показать расположение определенного устройства на карте.</span><span class="sxs-lookup"><span data-stu-id="48937-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="48937-106">Для использования этого действия необходимо, чтобы устройство iOS было в:</span><span class="sxs-lookup"><span data-stu-id="48937-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="48937-107">защищенном режиме;</span><span class="sxs-lookup"><span data-stu-id="48937-107">Supervised mode</span></span>
- <span data-ttu-id="48937-108">режиме пропажи.</span><span class="sxs-lookup"><span data-stu-id="48937-108">Lost mode</span></span>

<span data-ttu-id="48937-109">Дополнительные сведения см. в статье [Включить режим пропажи на устройствах с iOS и iPadOS с Intune](https://docs.microsoft.com/intune/device-lost-mode) и [Поиск потерянных или украденных устройств с iOS и iPadOS с Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="48937-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="48937-110">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="48937-110">**FAQ**</span></span>

<span data-ttu-id="48937-111">Вопрос. Я запустил удаленное действие для удаления данных компании с устройства, но оно зависло в состоянии ожидания.</span><span class="sxs-lookup"><span data-stu-id="48937-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="48937-112">Ответ. Для успешного выполнения удаленного действия целевое устройство должно быть подключено к сети и исправно.</span><span class="sxs-lookup"><span data-stu-id="48937-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="48937-113">В следующих ситуациях удаленное действие сохраняется в состоянии ожидания на 30 дней или до подтверждения команды на устройстве:</span><span class="sxs-lookup"><span data-stu-id="48937-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="48937-114">При отсутствии подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="48937-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="48937-115">При утрате состояния управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="48937-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="48937-116">Если вы считаете, что устройство больше не регистрируется и не сможет удалить данные компании, выберите "Удалить".</span><span class="sxs-lookup"><span data-stu-id="48937-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="48937-117">При удалении удаляется запись устройства, поэтому оно больше не отображается в списке устройств Intune.</span><span class="sxs-lookup"><span data-stu-id="48937-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="48937-118">Если устройство снова будет активным, то потребуется заново его зарегистрировать.</span><span class="sxs-lookup"><span data-stu-id="48937-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="48937-119">Вопрос. Почему некоторые удаленные действия недоступны для использования?</span><span class="sxs-lookup"><span data-stu-id="48937-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="48937-120">Ответ. Не все платформы поддерживают все удаленные действия с устройствами.</span><span class="sxs-lookup"><span data-stu-id="48937-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="48937-121">Указанные ниже удаленные действия можно использовать только для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="48937-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="48937-122">Обход блокировки активации (только iOS)</span><span class="sxs-lookup"><span data-stu-id="48937-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="48937-123">Начать заново (только Windows)</span><span class="sxs-lookup"><span data-stu-id="48937-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="48937-124">Режим утери (только iOS)</span><span class="sxs-lookup"><span data-stu-id="48937-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="48937-125">Обнаружить устройство (только iOS)</span><span class="sxs-lookup"><span data-stu-id="48937-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="48937-126">Перезапуск (только Windows)</span><span class="sxs-lookup"><span data-stu-id="48937-126">Restart (Windows only)</span></span>

<span data-ttu-id="48937-127">Дополнительные сведения о каждом из этих действий см. в статье [Доступные действия устройств](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="48937-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>