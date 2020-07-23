---
title: Конфликты с SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186128"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="075ab-102">Конфликты с SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="075ab-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="075ab-103">Если во время синхронизации появляются такие ошибки, как "В вашем каталоге уже существует синхронизированный объект с таким же ProxyAddress или UserPrincipalName", см. раздел [Диагностика и исправление ошибок синхронизации продублированных атрибутов](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="075ab-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="075ab-104">Кроме того, попробуйте включить устойчивость продублированных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="075ab-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="075ab-105">Дополнительные сведения см. в статье [Определение синхронизации и устойчивости продублированных атрибутов](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="075ab-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>