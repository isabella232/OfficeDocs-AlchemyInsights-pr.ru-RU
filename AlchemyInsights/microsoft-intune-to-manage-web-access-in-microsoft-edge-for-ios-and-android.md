---
title: Используйте Microsoft Intune для управления веб-доступом Microsoft Edge для iOS и Android
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
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989687"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="3a865-102">Используйте Microsoft Intune для управления веб-доступом Microsoft Edge для iOS и Android</span><span class="sxs-lookup"><span data-stu-id="3a865-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="3a865-103">Microsoft Edge для iOS и Android позволяет пользователю просматривать веб-страницы из нескольких совершенно отдельных профилей.</span><span class="sxs-lookup"><span data-stu-id="3a865-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="3a865-104">Самые широкие возможности защиты Microsoft 365 становятся доступными при подписке на пакет Enterprise Mobility + Security, который включает Microsoft Intune и Azure Active Directory Premium, например условный доступ.</span><span class="sxs-lookup"><span data-stu-id="3a865-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="3a865-105">Как минимум необходимо развернуть политику условного доступа, которая (1) позволяет пользователям подключаться с мобильных устройств к Microsoft Edge для iOS и Android и что (2) реализует политику защиты Microsoft Intune приложений, которая обеспечивает защищенную возможность просмотра.</span><span class="sxs-lookup"><span data-stu-id="3a865-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="3a865-106">Чтобы понять, как можно использовать условный доступ и политики, см. в рублях:</span><span class="sxs-lookup"><span data-stu-id="3a865-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="3a865-107">Применение Azure Active Directory политик условного доступа</span><span class="sxs-lookup"><span data-stu-id="3a865-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="3a865-108">Создание Microsoft Intune политик защиты приложений</span><span class="sxs-lookup"><span data-stu-id="3a865-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="3a865-109">Использование единого входного подключения для Azure Active Directory подключенных веб-приложений в браузерах, защищенных политикой</span><span class="sxs-lookup"><span data-stu-id="3a865-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="3a865-110">Использование конфигурации приложения для управления опытом просмотра</span><span class="sxs-lookup"><span data-stu-id="3a865-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="3a865-111">Разрешить использование только учетных записей для работы и учебных ок.</span><span class="sxs-lookup"><span data-stu-id="3a865-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="3a865-112">Развертывание общих политик конфигурации приложений</span><span class="sxs-lookup"><span data-stu-id="3a865-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="3a865-113">Развертывание политик конфигурации приложений для защиты данных</span><span class="sxs-lookup"><span data-stu-id="3a865-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="3a865-114">Использование Microsoft Endpoint Manager для развертывания политик конфигурации приложений</span><span class="sxs-lookup"><span data-stu-id="3a865-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="3a865-115">Подробнее о доступе к журналам управляемых приложений см. в Microsoft Edge для iOS и Android для доступа к журналам [управляемых приложений.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="3a865-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
