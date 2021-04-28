---
title: Проблемы с SharePoint на компьютерах с Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067001"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="26641-102">Проблемы с SharePoint на компьютерах с Windows 7</span><span class="sxs-lookup"><span data-stu-id="26641-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="26641-103">Если при работе с SharePoint или OneDrive на компьютерах с Windows 7 у вас возникают ошибки, они могут быть связаны с прекращением поддержки TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="26641-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="26641-104">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="26641-104">For more information, see:</span></span>

- [<span data-ttu-id="26641-105">Подготовка к TLS 1.2 в Office 365 и Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="26641-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="26641-106">В клиентах Windows 7 SP1 и Windows 8 должен быть включен протокол TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="26641-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="26641-107">Дополнительные сведения см. в статье [Возникновение ошибок проверки подлинности, если у клиента нет поддержки TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="26641-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="26641-108">Установите KB3140245 и создайте значение реестра.</span><span class="sxs-lookup"><span data-stu-id="26641-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="26641-109">Дополнительные сведения см. в статье  [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="26641-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="26641-110">В клиентах Windows 7 SP1 и Windows 8 должны быть установлены последние комплекты шифров TLS.</span><span class="sxs-lookup"><span data-stu-id="26641-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="26641-111">Дополнительные сведения см. в [советах корпорации Майкрософт по безопасности 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="26641-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


