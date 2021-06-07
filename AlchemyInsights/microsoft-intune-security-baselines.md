---
title: Используйте Microsoft Intune безопасности для настройки Windows 10 устройств
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783228"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="61ac5-102">Используйте Microsoft Intune безопасности для настройки Windows 10 устройств</span><span class="sxs-lookup"><span data-stu-id="61ac5-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="61ac5-103">Базовые конфигурации безопасности Intune помогают защитить пользователей и устройства.</span><span class="sxs-lookup"><span data-stu-id="61ac5-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="61ac5-104">Базовые показатели безопасности Windows предварительно настроенных групп, используемых для применения известной группы параметров и значений по умолчанию, рекомендуемых соответствующими группами безопасности.</span><span class="sxs-lookup"><span data-stu-id="61ac5-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="61ac5-105">Создавая профиль базовой конфигурации безопасности в Intune, вы создаете шаблон, состоящий из нескольких профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="61ac5-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="61ac5-106">При развертывании базовых показателей безопасности для групп пользователей или устройств эти параметры применяются к устройствам, которые работают на Windows 10 или позже.</span><span class="sxs-lookup"><span data-stu-id="61ac5-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="61ac5-107">Например, базовый уровень безопасности управления мобильными устройствами (MDM) Майкрософт автоматически включает BitLocker для съемных дисков, требует пароль для разблокировки устройства и отключает базовую проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="61ac5-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="61ac5-108">Если в вашей среде не поддерживается значение по умолчанию, вы можете настроить базовую конфигурацию, чтобы применить нужные параметры.</span><span class="sxs-lookup"><span data-stu-id="61ac5-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="61ac5-109">Базовые конфигурации безопасности также помогают создать комплексный безопасный рабочий процесс в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="61ac5-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="61ac5-110">Базовая конфигурация безопасности включает рекомендации для параметров, влияющих на безопасность.</span><span class="sxs-lookup"><span data-stu-id="61ac5-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="61ac5-111">Intune партнеров с группой Windows, которая создает базовые основы для групповой политики, поэтому эти рекомендации основаны на твердом руководстве и обширный опыт.</span><span class="sxs-lookup"><span data-stu-id="61ac5-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="61ac5-112">Если вы не знаете, с чего начать, базовые параметры безопасности помогут быстро создать и развернуть безопасный профиль.</span><span class="sxs-lookup"><span data-stu-id="61ac5-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="61ac5-113">Если вы в настоящее время используете групповую политику, миграция в Intune для целей управления намного проще с базовыми показателями безопасности, так как они встроены в Intune и включают передовые возможности управления.</span><span class="sxs-lookup"><span data-stu-id="61ac5-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="61ac5-114">Дополнительные данные см. [в Windows базовых показателей](/windows/security/threat-protection/windows-security-baselines) безопасности и [управления мобильными устройствами.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="61ac5-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

