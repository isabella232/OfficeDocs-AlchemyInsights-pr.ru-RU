---
title: Поведение Консистенцигуид и Саурцеанчор
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408121"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="2ce91-102">Поведение Консистенцигуид и Саурцеанчор</span><span class="sxs-lookup"><span data-stu-id="2ce91-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="2ce91-103">Azure AD Connect (версии 1.1.524.0 и After) теперь способствует использованию атрибута msDS-Консистенцигуид в качестве атрибута Саурцеанчор.</span><span class="sxs-lookup"><span data-stu-id="2ce91-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="2ce91-104">При использовании этой функции служба Azure AD Connect автоматически настраивает правила синхронизации следующим образом:</span><span class="sxs-lookup"><span data-stu-id="2ce91-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="2ce91-105">Используйте msDS — Консистенцигуид в качестве атрибута Саурцеанчор для объектов User.</span><span class="sxs-lookup"><span data-stu-id="2ce91-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="2ce91-106">ObjectGUID используется для других типов объектов.</span><span class="sxs-lookup"><span data-stu-id="2ce91-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="2ce91-107">Для любого объекта локального пользователя AD, чей атрибут msDS — Консистенцигуид не заполнен, Azure AD Connect записывает значение objectGUID обратно в атрибут msDS – Консистенцигуид в локальной службе Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ce91-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="2ce91-108">После заполнения атрибута msDS-Консистенцигуид Azure AD Connect затем экспортирует объект в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2ce91-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="2ce91-109">**Примечание:** После того как локальный объект AD импортируется в Azure AD Connect (то есть импортируется в пространство AD Connector и проецируется в метавселенной), его значение Саурцеанчор больше нельзя изменить.</span><span class="sxs-lookup"><span data-stu-id="2ce91-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="2ce91-110">Чтобы указать значение Саурцеанчор для данного локального объекта AD, настройте его атрибут msDS-Консистенцигуид перед его импортом в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2ce91-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="2ce91-111">Дополнительные сведения о Саурцеанчор и Консистенцигуид можно найти в следующих статьях: [Azure AD Connect: концепции дизайна](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="2ce91-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

