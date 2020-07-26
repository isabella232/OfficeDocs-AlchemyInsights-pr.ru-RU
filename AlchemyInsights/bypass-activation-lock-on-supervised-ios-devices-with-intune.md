---
title: Обход блокировки активации на защищенных устройствах iOS с помощью Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397759"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="e5f37-102">Обход блокировки активации на защищенных устройствах iOS с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="e5f37-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="e5f37-103">Возможность обхода блокировки активации на устройствах iOS упрощает восстановление в ситуации, когда пользователь включает блокировку активации на корпоративном устройстве, а затем увольняется из компании.</span><span class="sxs-lookup"><span data-stu-id="e5f37-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="e5f37-104">Необходимые условия для обхода блокировки активации:</span><span class="sxs-lookup"><span data-stu-id="e5f37-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="e5f37-105">Устройство должно быть "защищено".</span><span class="sxs-lookup"><span data-stu-id="e5f37-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="e5f37-106">Блокировка активации должна быть успешно включена с помощью политики ограничений устройства iOS в Intune.</span><span class="sxs-lookup"><span data-stu-id="e5f37-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="e5f37-107">Кроме того, при обходе блокировки активации необходимо:</span><span class="sxs-lookup"><span data-stu-id="e5f37-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="e5f37-108">Физически владеть устройством, на котором выполняется очистка.</span><span class="sxs-lookup"><span data-stu-id="e5f37-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="e5f37-109">Скопировать код перед началом очистки.</span><span class="sxs-lookup"><span data-stu-id="e5f37-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="e5f37-110">**Примечание.** В коде очистки не учитывается регистр, поэтому символы "-" не требуются.</span><span class="sxs-lookup"><span data-stu-id="e5f37-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="e5f37-111">Дополнительные сведения см. в статье [Обход блокировки активации на защищенных устройствах iOS с помощью Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="e5f37-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="e5f37-112">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="e5f37-112">**FAQ**</span></span>

<span data-ttu-id="e5f37-113">Вопрос. **Я запустил удаленное действие для удаления данных компании с устройства, но оно зависло в состоянии ожидания.**</span><span class="sxs-lookup"><span data-stu-id="e5f37-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="e5f37-114">Ответ. Для успешного выполнения удаленного действия целевое устройство должно быть подключено к сети и исправно.</span><span class="sxs-lookup"><span data-stu-id="e5f37-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="e5f37-115">В следующих ситуациях удаленное действие сохраняется в состоянии ожидания на 30 дней или до подтверждения команды на устройстве:</span><span class="sxs-lookup"><span data-stu-id="e5f37-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="e5f37-116">Нет подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="e5f37-116">Does not have connectivity.</span></span>
- <span data-ttu-id="e5f37-117">Утрачено состояние управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="e5f37-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="e5f37-118">Если вы считаете, что устройство больше не регистрируется и не удалит данные компании, выберите "Удалить".</span><span class="sxs-lookup"><span data-stu-id="e5f37-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="e5f37-119">При удалении удаляется запись устройства, поэтому оно больше не отображается в списке устройств Intune.</span><span class="sxs-lookup"><span data-stu-id="e5f37-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="e5f37-120">Чтобы это устройство снова стало активным, пользователь должен повторно зарегистрировать его.</span><span class="sxs-lookup"><span data-stu-id="e5f37-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="e5f37-121">Вопрос. **Почему некоторые удаленные действия недоступны для использования?**</span><span class="sxs-lookup"><span data-stu-id="e5f37-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="e5f37-122">Ответ. Не все платформы поддерживают все удаленные действия с устройствами.</span><span class="sxs-lookup"><span data-stu-id="e5f37-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="e5f37-123">Следующие удаленные действия зависят от платформы.</span><span class="sxs-lookup"><span data-stu-id="e5f37-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="e5f37-124">Обход блокировки активации (только iOS)</span><span class="sxs-lookup"><span data-stu-id="e5f37-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="e5f37-125">Начать заново (только Windows)</span><span class="sxs-lookup"><span data-stu-id="e5f37-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="e5f37-126">Режим утери (только iOS)</span><span class="sxs-lookup"><span data-stu-id="e5f37-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="e5f37-127">Обнаружить устройство (только iOS)</span><span class="sxs-lookup"><span data-stu-id="e5f37-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="e5f37-128">Перезапуск (только Windows)</span><span class="sxs-lookup"><span data-stu-id="e5f37-128">Restart (Windows only)</span></span>

<span data-ttu-id="e5f37-129">Дополнительные сведения о каждом из этих действий см. в статье [Доступные действия устройств](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="e5f37-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>