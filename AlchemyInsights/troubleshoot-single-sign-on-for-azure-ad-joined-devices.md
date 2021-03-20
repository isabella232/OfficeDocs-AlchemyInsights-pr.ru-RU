---
title: Устранение неполадок с одним входом для устройств, присоединитых к Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898086"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="fe78a-102">Устранение неполадок с одним входом для устройств, присоединитых к Azure AD</span><span class="sxs-lookup"><span data-stu-id="fe78a-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="fe78a-103">Если у вас есть локальное окружение Active Directory (AD) и вы хотите присоединиться к компьютерам, присоединимым к домену AD, в Azure AD, вы можете добиться этого путем гибридного пользования Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe78a-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="fe78a-104">[Как: планирование реализации](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) гибридного реализации Azure Active Directory предоставляет вам соответствующие действия по реализации гибридного присоединиться к Azure AD в вашей среде.</span><span class="sxs-lookup"><span data-stu-id="fe78a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="fe78a-105">Дополнительные сведения см. в видеоролике [Configure Azure AD joined devices for on-premises Single-Sign On using Windows Hello for Business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="fe78a-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="fe78a-106">**Основные проблемы маркера обновления (PRT)**</span><span class="sxs-lookup"><span data-stu-id="fe78a-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="fe78a-107">Основной маркер обновления (PRT) — это ключевой артефакт проверки подлинности Azure AD на устройствах Windows 10, Windows Server 2016 и более поздних версий, iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="fe78a-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="fe78a-108">Это веб-маркер JSON (JWT), специально выданный брокерам маркеров первой стороны Майкрософт, чтобы включить единую регистрацию (SSO) в приложениях, используемых на этих устройствах.</span><span class="sxs-lookup"><span data-stu-id="fe78a-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="fe78a-109">Сведения о том, как prT выдают, используют и защищают на устройствах с Windows 10, см. в материале [What is a Primary Refresh Token?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="fe78a-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="fe78a-110">**WamDefaultSet: ДА и AzureADPrt: ДА**</span><span class="sxs-lookup"><span data-stu-id="fe78a-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="fe78a-111">В этих полях указывается, успешно ли пользователь прошел проверку подлинности в Azure AD при входе на устройство.</span><span class="sxs-lookup"><span data-stu-id="fe78a-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="fe78a-112">Если значения **нет,** это может быть связано с:</span><span class="sxs-lookup"><span data-stu-id="fe78a-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="fe78a-113">Плохой ключ хранения в TPM, связанный с устройством при регистрации (проверьте KeySignTest при работе с повышенным значением)</span><span class="sxs-lookup"><span data-stu-id="fe78a-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="fe78a-114">Альтернативный ID входа</span><span class="sxs-lookup"><span data-stu-id="fe78a-114">Alternate Login ID</span></span>
- <span data-ttu-id="fe78a-115">Http Proxy не найден</span><span class="sxs-lookup"><span data-stu-id="fe78a-115">HTTP Proxy not found</span></span>

<span data-ttu-id="fe78a-116">Для устранения неполадок устройств с помощью команды dsregcmd см. [состояние SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="fe78a-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
