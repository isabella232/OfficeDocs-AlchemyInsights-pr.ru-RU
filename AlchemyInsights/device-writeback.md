---
title: Переописка устройства
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255173"
---
# <a name="device-writeback"></a><span data-ttu-id="b1156-102">Переописка устройства</span><span class="sxs-lookup"><span data-stu-id="b1156-102">Device Writeback</span></span>

<span data-ttu-id="b1156-103">Переописка устройства используется в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="b1156-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="b1156-104">Включить [Windows Hello для бизнеса с помощью гибридного развертывания с доверием на сертификаты](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="b1156-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="b1156-105">Включить условный доступ на основе устройств в защищенных приложениях ADFS (2012 R2 или более высоких) (отношения доверия с отношениями</span><span class="sxs-lookup"><span data-stu-id="b1156-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="b1156-106">Для записи устройств необходима подписка на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="b1156-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="b1156-107">Это обеспечивает дополнительную безопасность и гарантии того, что доступ к приложениям предоставляется только доверенным устройствам.</span><span class="sxs-lookup"><span data-stu-id="b1156-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="b1156-108">Дополнительные сведения об условном [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) доступе см. в под управлением рисками с помощью условного доступа и настройке локального условного доступа с помощью [службы регистрации устройств Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="b1156-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="b1156-109">Дополнительные сведения о включаемой записи устройства для устройств см. в этой [теме.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="b1156-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
