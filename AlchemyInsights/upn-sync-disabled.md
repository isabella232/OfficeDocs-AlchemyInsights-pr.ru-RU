---
title: Синхронизация имени участника-пользователя отключена
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532344"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="7f09e-102">Синхронизация имени участника-пользователя отключена</span><span class="sxs-lookup"><span data-stu-id="7f09e-102">UPN sync disabled</span></span>

<span data-ttu-id="7f09e-103">Если вы начали синхронизацию с Azure AD до 30 марта 2016, запустите следующий командлет Azure AD PowerShell, чтобы включить мягкое обновление имени участника-пользователя только для вашей организации:</span><span class="sxs-lookup"><span data-stu-id="7f09e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="7f09e-104">**Set – Мсолдирсинкфеатуре — Feature Енаблесофтматчонупн — Enable $True**</span><span class="sxs-lookup"><span data-stu-id="7f09e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="7f09e-105">Мягкое обновление UPN автоматически включается для организаций, которые начали синхронизироваться с Azure AD на или после 30 марта 2016 г.</span><span class="sxs-lookup"><span data-stu-id="7f09e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="7f09e-106">Чтобы узнать больше о том, как включить мягкое сравнение на UPN и других функциях синхронизации, обратитесь к разделу [функции службы синхронизации Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="7f09e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

