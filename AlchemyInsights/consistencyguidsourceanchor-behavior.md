---
title: ConsistencyGuid / sourceAnchor behaviour
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817005"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behaviour

Azure AD Connect (версия 1.1.524.0 и после) теперь упрощает использование msDS-ConsistencyGuid в качестве атрибута sourceAnchor. При использовании этой функции Azure AD Connect автоматически настраивает правила синхронизации на:
  
- Используйте msDS-ConsistencyGuid в качестве атрибута sourceAnchor для объектов пользователя. ObjectGUID используется для других типов объектов.
    
- Для любого локального объекта AD User, атрибут msDS-ConsistencyGuid которого не заполнен, Azure AD Connect записывает свое значение objectGUID обратно в атрибут msDS-ConsistencyGuid в локальном Active Directory. После заполнения атрибута msDS-ConsistencyGuid Azure AD Connect экспортирует объект в Azure AD.
    
 **Примечание:** После импорта локального объекта AD в Azure AD Connect (то есть импортируемого в пространство соединителя AD и проецируемого в Metaverse), невозможно изменить его значение sourceAnchor. Чтобы указать значение sourceAnchor для данного локального объекта AD, настройте атрибут msDS-ConsistencyGuid перед его импортом в Azure AD Connect. 
  
Дополнительные сведения о SourceAnchor и ConsistencyGuid можно найти в следующих сведениях: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

