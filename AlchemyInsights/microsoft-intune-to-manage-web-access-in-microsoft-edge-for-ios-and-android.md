---
title: Использование Microsoft Intune для управления веб-доступом в Microsoft Edge для iOS и Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617340"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="d5637-102">Использование Microsoft Intune для управления веб-доступом в Microsoft Edge для iOS и Android</span><span class="sxs-lookup"><span data-stu-id="d5637-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="d5637-103">Microsoft Edge для iOS и Android позволяет пользователю просматривать веб-страницы из нескольких совершенно разных профилей.</span><span class="sxs-lookup"><span data-stu-id="d5637-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="d5637-104">Самые широкие возможности защиты для данных Microsoft 365 становятся доступны при подписке на набор Enterprise Mobility + Security, который включает функции Microsoft Intune и Azure Active Directory Premium, такие как условный доступ.</span><span class="sxs-lookup"><span data-stu-id="d5637-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="d5637-105">Вам, как минимум, нужно развернуть политику условного доступа, которая (1) позволяет пользователям подключаться с мобильных устройств к Microsoft Edge для iOS и Android и (2) реализует политику защиты приложений Microsoft Intune, которая обеспечивает защищенный просмотр.</span><span class="sxs-lookup"><span data-stu-id="d5637-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="d5637-106">Чтобы понять, как можно использовать условный доступ и политики, см. статью:</span><span class="sxs-lookup"><span data-stu-id="d5637-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="d5637-107">Применение политик условного доступа Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d5637-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="d5637-108">Создание политик защиты приложений Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d5637-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="d5637-109">Использование единого вход для веб-приложений, подключенных к Azure Active Directory, в браузерах, защищенных политикой</span><span class="sxs-lookup"><span data-stu-id="d5637-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="d5637-110">Использование конфигурации приложения для управления просмотром</span><span class="sxs-lookup"><span data-stu-id="d5637-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="d5637-111">Разрешить использование только учетных записей для работы и учебного заведения</span><span class="sxs-lookup"><span data-stu-id="d5637-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="d5637-112">Развертывание общих политик конфигурации приложений</span><span class="sxs-lookup"><span data-stu-id="d5637-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="d5637-113">Развертывание политик конфигурации приложений для защиты данных</span><span class="sxs-lookup"><span data-stu-id="d5637-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="d5637-114">Развертывание политик конфигурации приложений с помощью Microsoft Endpoint Manager</span><span class="sxs-lookup"><span data-stu-id="d5637-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="d5637-115">Чтобы узнать, как получить доступ к журналам управляемых приложений, см. microsoft Edge для iOS и Android для доступа [к журналам управляемых приложений.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="d5637-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
