---
title: Single-Sign для устройств Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403830"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="02940-102">Единый вход для устройств, присоединив к Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="02940-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="02940-103">Если у вас есть локальное окружение Active Directory (AD) и вы хотите присоединиться к компьютерам, присоединимым к домену AD, в Azure AD, вы можете добиться этого путем гибридного пользования Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02940-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="02940-104">[Как: планирование реализации](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) гибридного реализации Azure Active Directory предоставляет вам соответствующие действия по реализации гибридного присоединиться к Azure AD в вашей среде.</span><span class="sxs-lookup"><span data-stu-id="02940-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="02940-105">Настройка устройств Azure AD для локального Single-Sign с помощью Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="02940-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="02940-106">**Основные проблемы маркера обновления (PRT)** Основной маркер обновления (PRT) — это ключевой артефакт проверки подлинности Azure AD на устройствах Windows 10, Windows Server 2016 и более поздних версий, iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="02940-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="02940-107">Это веб-маркер JSON (JWT), специально выданный брокерам маркеров первой стороны Майкрософт, чтобы включить единую регистрацию (SSO) в приложениях, используемых на этих устройствах.</span><span class="sxs-lookup"><span data-stu-id="02940-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="02940-108">[В "Что такое основной маркер обновления?",](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)мы предокажим сведения о том, как prT выдают, используют и защищают на устройствах с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="02940-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="02940-109">**WamDefaultSet: ДА и AzureADPrt: ДА** В этих полях указывается, успешно ли пользователь прошел проверку подлинности в Azure AD при входе на устройство.</span><span class="sxs-lookup"><span data-stu-id="02940-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="02940-110">Если значения **нет,** это может быть связано:</span><span class="sxs-lookup"><span data-stu-id="02940-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="02940-111">Плохой ключ хранилища в TPM, связанный с устройством при регистрации (проверьте KeySignTest при работе с повышенным значением).</span><span class="sxs-lookup"><span data-stu-id="02940-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="02940-112">Альтернативный ID входа</span><span class="sxs-lookup"><span data-stu-id="02940-112">Alternate Login ID</span></span>
- <span data-ttu-id="02940-113">Http Proxy не найден</span><span class="sxs-lookup"><span data-stu-id="02940-113">HTTP Proxy not found</span></span>

<span data-ttu-id="02940-114">Устройства устранения неполадок с помощью команды dsregcmd - [состояние SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="02940-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
