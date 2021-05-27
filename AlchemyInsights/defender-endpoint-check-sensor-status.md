---
title: Defender для конечной точки — проверка состояния датчиков
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627242"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="c9289-102">Defender для конечной точки — проверка состояния датчиков</span><span class="sxs-lookup"><span data-stu-id="c9289-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="c9289-103">Плитка **Устройства с проблемами датчиков** находится на панели мониторинга операций безопасности.</span><span class="sxs-lookup"><span data-stu-id="c9289-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="c9289-104">На этой плитке содержатся сведения о способности отдельного устройства предоставлять данные датчиков и обмениваться информаций со службой Defender для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="c9289-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="c9289-105">На этой плитке указано, скольким устройствам требуется внимание. Вы можете удобно выявлять проблемные устройства и принимать меры для устранения известных проблем.</span><span class="sxs-lookup"><span data-stu-id="c9289-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="c9289-106">Два индикатора состояния на этой плитке предоставляют сведения о количестве устройств, от которых информация не поступает в службу должным образом:</span><span class="sxs-lookup"><span data-stu-id="c9289-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="c9289-107">**Неверная конфигурация**: устройства, передающие неполные данные датчиков в службу Defender для конечной точки. На таких устройствах могут быть ошибки конфигурации, нуждающиеся в исправлении. </span><span class="sxs-lookup"><span data-stu-id="c9289-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="c9289-108">**Неактивные**: устройства, переставшие передавать данные в службу Defender для конечной точки как минимум в течение семи дней в прошлом месяце.</span><span class="sxs-lookup"><span data-stu-id="c9289-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="c9289-109">Щелкните любую группу, чтобы перейти в список "Устройства", отфильтрованный в соответствии с вашими предпочтениями.</span><span class="sxs-lookup"><span data-stu-id="c9289-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="c9289-110">В списке устройств можно отфильтровать список состояния работоспособности по следующему состоянию:</span><span class="sxs-lookup"><span data-stu-id="c9289-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="c9289-111">**Активные**: устройства, активно передающие данные в службу Defender для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="c9289-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="c9289-112">**Неверная конфигурация**: устройства, передающие неполные данные датчиков в службу Defender для конечной точки. На таких устройствах могут быть ошибки конфигурации, нуждающиеся в исправлении. </span><span class="sxs-lookup"><span data-stu-id="c9289-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="c9289-113">На устройствах с неверной конфигурацией могут быть следующие проблемы (как по отдельности, так и вместе):</span><span class="sxs-lookup"><span data-stu-id="c9289-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="c9289-114">Нет данных датчиков — устройства прекратили отправлять данные датчиков.</span><span class="sxs-lookup"><span data-stu-id="c9289-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="c9289-115">С устройства можно инициировать ограниченный набор оповещений.</span><span class="sxs-lookup"><span data-stu-id="c9289-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="c9289-116">Нарушение связи: нарушена возможность обмена данными с устройством.</span><span class="sxs-lookup"><span data-stu-id="c9289-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="c9289-117">При этом могут не работать такие функции как отправка файлов для подробного анализа, блокирование файлов, изоляция устройства от сети, а также другие действия, для которых требуется обмен информацией с устройством.</span><span class="sxs-lookup"><span data-stu-id="c9289-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="c9289-118">**Неактивные**: устройства, переставшие передавать данные в службу Defender для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="c9289-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="c9289-119">Вы можете скачать весь список в формате CSV с помощью функции экспорта.</span><span class="sxs-lookup"><span data-stu-id="c9289-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="c9289-120">Дополнительные сведения см. в статье [Проверка состояния работоспособности датчиков в Microsoft Defender для конечной точки](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="c9289-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="c9289-121">Дополнительные сведения о причинах неактивности и неправильной настройки устройств см. в статье [Исправление неработоспособных датчиков в Microsoft Defender для конечной точки](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="c9289-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
