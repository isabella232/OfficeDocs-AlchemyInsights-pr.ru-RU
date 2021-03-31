---
title: EndPoint Manager — базовые конфигурации безопасности
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440897"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="f6745-102">EndPoint Manager — базовые конфигурации безопасности</span><span class="sxs-lookup"><span data-stu-id="f6745-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="f6745-103">Базовые конфигурации безопасности — это предварительно настроенные группы параметров Windows, помогающие применять параметры безопасности, рекомендуемые соответствующими командами безопасности.</span><span class="sxs-lookup"><span data-stu-id="f6745-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="f6745-104">Эти базовые конфигурации можно настроить для предоставления только нужных параметров и значений.</span><span class="sxs-lookup"><span data-stu-id="f6745-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="f6745-105">Дополнительные сведения о базовых конфигурациях безопасности см. в статье [Использование базовых конфигураций безопасности для настройки устройств с Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="f6745-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="f6745-106">В настоящее время существуют базовые конфигурации для следующих продуктов.</span><span class="sxs-lookup"><span data-stu-id="f6745-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="f6745-107">Параметры безопасности Windows MDM</span><span class="sxs-lookup"><span data-stu-id="f6745-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="f6745-108">Параметры Microsoft Defender для конечной точки</span><span class="sxs-lookup"><span data-stu-id="f6745-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="f6745-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f6745-109">Microsoft Edge</span></span>

<span data-ttu-id="f6745-110">Каждая из этих базовых конфигураций периодически обновляется и выпускается в добавочных версиях.</span><span class="sxs-lookup"><span data-stu-id="f6745-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="f6745-111">Каждая версия добавляет и (или) удаляет параметры из предыдущей версии, чтобы базовая конфигурация соответствовала текущим рекомендациям.</span><span class="sxs-lookup"><span data-stu-id="f6745-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="f6745-112">Консоль базовых конфигураций безопасности в Безопасности конечной точки позволяет сравнивать разные версии, отображая изменения, внесенные в версиях.</span><span class="sxs-lookup"><span data-stu-id="f6745-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="f6745-113">Инструкции по наиболее эффективному изменению развертываемой версии базовой конфигурации см. в статье [Управление профилями базовых конфигураций безопасности в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="f6745-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="f6745-114">После развертывания базовой конфигурации безопасности вы можете отслеживать состояние развертывания и просматривать параметры для отдельных устройств.</span><span class="sxs-lookup"><span data-stu-id="f6745-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="f6745-115">**Примечание.** Отображение данных отчетов для базовых конфигураций может занять до 24 часов после начального развертывания на устройстве и до 6 часов для последующих обновлений.</span><span class="sxs-lookup"><span data-stu-id="f6745-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="f6745-116">Наиболее распространенной причиной, по которой не применяется параметр базовой конфигурации, является то, что этот параметр используется в другом профиле.</span><span class="sxs-lookup"><span data-stu-id="f6745-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="f6745-117">Этот сценарий можно исследовать для конкретного устройства, выбрав это устройство в узле "Состояние устройства" профиля базовой конфигурации безопасности.</span><span class="sxs-lookup"><span data-stu-id="f6745-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="f6745-118">Подробные сведения см. в разделе [Разрешение конфликтов для базовых конфигураций безопасности](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="f6745-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>