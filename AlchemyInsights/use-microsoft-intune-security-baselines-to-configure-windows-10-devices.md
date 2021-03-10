---
title: Использование базовых конфигураций безопасности Microsoft Intune для настройки устройств с Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641627"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="4d3db-102">Использование базовых конфигураций безопасности Microsoft Intune для настройки устройств с Windows 10</span><span class="sxs-lookup"><span data-stu-id="4d3db-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="4d3db-103">Базовые конфигурации безопасности Intune помогают защитить пользователей и устройства.</span><span class="sxs-lookup"><span data-stu-id="4d3db-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="4d3db-104">Базовые конфигурации безопасности — это предварительно настроенные группы параметров Windows, используемые для применения известной группы параметров и значений по умолчанию, рекомендуемых соответствующими командами безопасности.</span><span class="sxs-lookup"><span data-stu-id="4d3db-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="4d3db-105">Создавая профиль базовой конфигурации безопасности в Intune, вы создаете шаблон, состоящий из нескольких профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="4d3db-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="4d3db-106">Когда вы разворачиваете базовые конфигурации безопасности для групп пользователей или устройств, эти параметры применяются к устройствам под управлением Windows 10 или более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="4d3db-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="4d3db-107">Например, базовая конфигурация безопасности управления мобильными устройствами (MDM) Майкрософт автоматически (1) включает BitLocker для съемных дисков, (2) требует пароля для разблокировки устройства и (3) отключает обычную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="4d3db-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="4d3db-108">Если в вашей среде не поддерживается значение по умолчанию, вы можете настроить базовую конфигурацию, чтобы применить нужные параметры.</span><span class="sxs-lookup"><span data-stu-id="4d3db-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="4d3db-109">Базовые конфигурации безопасности также помогают создать комплексный безопасный рабочий процесс в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4d3db-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="4d3db-110">Вот некоторые преимущества этой функции:</span><span class="sxs-lookup"><span data-stu-id="4d3db-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="4d3db-111">Базовая конфигурация безопасности включает рекомендации для параметров, влияющих на безопасность.</span><span class="sxs-lookup"><span data-stu-id="4d3db-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="4d3db-112">Так как Intune взаимодействует с командой безопасности Windows, создающей базовые конфигурации для групповых политик, эти рекомендации основаны на надежных руководствах и обширном опыте.</span><span class="sxs-lookup"><span data-stu-id="4d3db-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="4d3db-113">Если вы не работали в Intune или не знаете, с чего начать, базовые конфигурации безопасности помогут вам быстро создать и развернуть безопасный профиль.</span><span class="sxs-lookup"><span data-stu-id="4d3db-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="4d3db-114">Если вы используете групповую политику, миграция в Intune в целях управления значительно упрощается с помощью базовых конфигураций безопасности, так как эти базовые конфигурации безопасности встроены в Intune и включают новейшие возможности управления.</span><span class="sxs-lookup"><span data-stu-id="4d3db-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="4d3db-115">Дополнительные сведения см. в статьях [Базовые конфигурации безопасности Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) и [Управление мобильными устройствами](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="4d3db-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>