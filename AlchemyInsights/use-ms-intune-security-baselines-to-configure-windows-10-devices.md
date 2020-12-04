---
title: Настройка устройств с Windows 10 с помощью базовых планов безопасности Microsoft Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571895"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="53f28-102">Настройка устройств с Windows 10 с помощью базовых планов безопасности Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53f28-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="53f28-103">Базовые показатели безопасности Intune помогают защитить пользователей и устройства.</span><span class="sxs-lookup"><span data-stu-id="53f28-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="53f28-104">Базовые планы безопасности — это предварительно настроенные группы параметров Windows, которые использовались для применения известной группы параметров и значений по умолчанию, рекомендуемых соответствующими группами обеспечения безопасности.</span><span class="sxs-lookup"><span data-stu-id="53f28-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="53f28-105">Создавая базовый профиль безопасности в Intune, вы создаете шаблон, который состоит из нескольких профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="53f28-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="53f28-106">При развертывании базовых показателей безопасности до групп пользователей или устройств эти параметры применяются к устройствам, которые работают в Windows 10 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="53f28-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="53f28-107">Например, базовый план безопасности MDM автоматически (1) включает BitLocker для съемных дисков, (2) требует пароль для разблокировки устройства, а (3) отключает обычную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="53f28-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="53f28-108">Если значение по умолчанию не работает в вашей среде, настройте базовую линию для применения нужных параметров.</span><span class="sxs-lookup"><span data-stu-id="53f28-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="53f28-109">Шаблоны безопасности также помогают установить сквозной безопасный рабочий процесс в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="53f28-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="53f28-110">Ниже приведены некоторые преимущества.</span><span class="sxs-lookup"><span data-stu-id="53f28-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="53f28-111">Базовый план безопасности содержит рекомендации и рекомендации для параметров, влияющих на безопасность.</span><span class="sxs-lookup"><span data-stu-id="53f28-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="53f28-112">Так как партнеры Intune с группой безопасности Windows, которая создает базовые планы для групповых политик, эти рекомендации основываются на надежном руководстве и расширенном интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="53f28-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="53f28-113">Если вы не знакомы с Intune и не знаете, с чего начать, базовые планы безопасности помогут быстро создать и развернуть защищенный профиль.</span><span class="sxs-lookup"><span data-stu-id="53f28-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="53f28-114">Если в настоящее время используется групповая политика, то миграция в Intune в целях управления значительно упрощается с учетом базовых показателей безопасности, так как они встроены в Intune и включают в себя новейшие возможности управления.</span><span class="sxs-lookup"><span data-stu-id="53f28-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="53f28-115">Чтобы узнать больше, ознакомьтесь с [планами безопасности Windows](https://go.microsoft.com/fwlink/?linkid=2141503) и [управлением мобильными устройствами](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="53f28-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>