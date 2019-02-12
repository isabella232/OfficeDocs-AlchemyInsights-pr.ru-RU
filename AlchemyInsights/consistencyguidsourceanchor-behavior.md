---
title: ConsistencyGuid / sourceAnchor поведение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927685"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor поведение

Подключение Azure AD (версия 1.1.524.0 и после) теперь упрощает использование msDS-ConsistencyGuid в качестве атрибута sourceAnchor. При использовании этой функции, Azure AD подключение автоматически настраивает правила синхронизации для:
  
- Используйте msDS-ConsistencyGuid в качестве атрибута sourceAnchor для объектов-пользователей. ObjectGUID используется для других типов объектов.
    
- Для любой заданной локального пользователя AD объект, чьи атрибута msDS-ConsistencyGuid не заполненной, Azure операций записи AD подключить его значение objectGUID обратно атрибута msDS-ConsistencyGuid в локальной службе Active Directory. После заполнения атрибута msDS-ConsistencyGuid Azure AD подключение выберите Экспорт объекта Azure AD.
    
 **Примечание:** Один раз локальный объект AD, импортированные в Azure AD подключение (то есть импортированные в пространство соединителя AD и проекции в метавселенной), не может изменить его значение sourceAnchor больше. Чтобы указать значение sourceAnchor для присвоенное локальной AD, следует настроить его атрибута msDS-ConsistencyGuid до его импорта в Azure AD подключение. 
  
Дополнительные сведения о SourceAnchor и ConsistencyGuid см: [Azure AD Connect: Разработка концепции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

