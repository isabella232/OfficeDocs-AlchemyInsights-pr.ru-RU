---
title: Учет Устройств Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434635"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="d4364-102">Учет Устройств Intune</span><span class="sxs-lookup"><span data-stu-id="d4364-102">Intune Device Inventory</span></span>

<span data-ttu-id="d4364-103">Раздел "Устройства" позволяет администратору получить информацию по каждому устройству, находящемуся под управлением в Intune.</span><span class="sxs-lookup"><span data-stu-id="d4364-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="d4364-104">Представленная информация включает в себя: оборудование, обнаруженные приложения, состояние соответствия условиям политики и состояние конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4364-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="d4364-105">Результаты инвентаризации для оборудования и информация об обнаруженных приложениях собираются в течение семи дней.</span><span class="sxs-lookup"><span data-stu-id="d4364-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="d4364-106">Приложения и конкретные элементы оборудования различаются в зависимости от операционной системы устройства и от того, является ли это устройство личным или корпоративным.</span><span class="sxs-lookup"><span data-stu-id="d4364-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="d4364-107">Дополнительные сведения см. в разделе[Сведения об устройстве в Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="d4364-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="d4364-108">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="d4364-108">**FAQ**</span></span>

<span data-ttu-id="d4364-109">Вопрос: мне не удается получить полный инвентарный список приложений, присутствующих на устройствах с Windows, зарегистрированных в Intune.</span><span class="sxs-lookup"><span data-stu-id="d4364-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="d4364-110">Почему нет?</span><span class="sxs-lookup"><span data-stu-id="d4364-110">Why not?</span></span>

<span data-ttu-id="d4364-111">Ответ: В настоящее время только современные приложения включены в список для ПК с Windows 10, которые обозначены как корпоративные устройства.</span><span class="sxs-lookup"><span data-stu-id="d4364-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="d4364-112">Intune не собирает сведения о приложениях Win32, установленных на этих устройствах.</span><span class="sxs-lookup"><span data-stu-id="d4364-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="d4364-113">Вопрос: Почему номера телефонов не собираются со всех устройств?</span><span class="sxs-lookup"><span data-stu-id="d4364-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="d4364-114">Ответ: Телефоны, отнесенные к категории корпоративных устройств в Intune, не идентифицируются с их полным номером телефона, например, когда вы запускаете отчет об инвентаризации мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="d4364-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="d4364-115">Телефонные номера устройств всегда частично замаскированы звездочками (\*\*\*\*), и показываются только последние четыре цифры.</span><span class="sxs-lookup"><span data-stu-id="d4364-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>