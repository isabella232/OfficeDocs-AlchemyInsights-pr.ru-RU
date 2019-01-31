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
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659604"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor поведение

Подключение Azure AD (версия 1.1.524.0 и после) теперь упрощает использование msDS-ConsistencyGuid в качестве атрибута sourceAnchor. При использовании этой функции, Azure AD подключение автоматически настраивает правила синхронизации для:
  
- Используйте msDS-ConsistencyGuid в качестве атрибута sourceAnchor для объектов-пользователей. ObjectGUID используется для других типов объектов.
    
- Для любой заданной локального пользователя AD объект, чьи атрибута msDS-ConsistencyGuid не заполненной, Azure операций записи AD подключить его значение objectGUID обратно атрибута msDS-ConsistencyGuid в локальной службе Active Directory. После заполнения атрибута msDS-ConsistencyGuid Azure AD подключение выберите Экспорт объекта Azure AD.
    
 **Примечание:** Один раз локальный объект AD, импортированные в Azure AD подключение (то есть импортированные в пространство соединителя AD и проекции в метавселенной), не может изменить его значение sourceAnchor больше. Чтобы указать значение sourceAnchor для присвоенное локальной AD, следует настроить его атрибута msDS-ConsistencyGuid до его импорта в Azure AD подключение. 
  
Дополнительные сведения о SourceAnchor и ConsistencyGuid см: [Azure AD Connect: Разработка концепции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

