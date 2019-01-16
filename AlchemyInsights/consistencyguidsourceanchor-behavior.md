---
title: ConsistencyGuid / sourceAnchor поведение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308215"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f580d-102">ConsistencyGuid / sourceAnchor поведение</span><span class="sxs-lookup"><span data-stu-id="f580d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f580d-p101">Подключение Azure AD (версия 1.1.524.0 и после) теперь упрощает использование msDS-ConsistencyGuid в качестве атрибута sourceAnchor. При использовании этой функции, Azure AD подключение автоматически настраивает правила синхронизации для:</span><span class="sxs-lookup"><span data-stu-id="f580d-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f580d-p102">Используйте msDS-ConsistencyGuid в качестве атрибута sourceAnchor для объектов-пользователей. ObjectGUID используется для других типов объектов.</span><span class="sxs-lookup"><span data-stu-id="f580d-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f580d-p103">Для любой заданной локального пользователя AD объект, чьи атрибута msDS-ConsistencyGuid не заполненной, Azure операций записи AD подключить его значение objectGUID обратно атрибута msDS-ConsistencyGuid в локальной службе Active Directory. После заполнения атрибута msDS-ConsistencyGuid Azure AD подключение выберите Экспорт объекта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f580d-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f580d-p104">**Примечание:** Один раз локальный объект AD, импортированные в Azure AD подключение (то есть импортированные в пространство соединителя AD и проекции в метавселенной), не может изменить его значение sourceAnchor больше. Чтобы указать значение sourceAnchor для присвоенное локальной AD, следует настроить его атрибута msDS-ConsistencyGuid до его импорта в Azure AD подключение.</span><span class="sxs-lookup"><span data-stu-id="f580d-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f580d-111">Дополнительные сведения о SourceAnchor и ConsistencyGuid см: [Azure AD Connect: Разработка концепции](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f580d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

