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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044353"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behaviour

Azure AD Подключение (версия 1.1.524.0 и после) теперь упрощает использование msDS-ConsistencyGuid в качестве атрибута sourceAnchor. При использовании этой функции Azure AD Подключение автоматически настраивает правила синхронизации на:
  
- Используйте msDS-ConsistencyGuid в качестве атрибута sourceAnchor для объектов пользователя. ObjectGUID используется для других типов объектов.
    
- Для любого локального объекта AD User, атрибут msDS-ConsistencyGuid которого не заполнен, Azure AD Подключение записывает свое значение objectGUID обратно в атрибут msDS-ConsistencyGuid в локальном Active Directory. После заполнения атрибута msDS-ConsistencyGuid Azure AD Подключение затем экспортирует объект в Azure AD.
    
 **Примечание:** После импорта локального объекта AD в Azure AD Подключение (то есть импортируется в пространство соединителя AD и проецируется в Metaverse), изменить его значение sourceAnchor больше нельзя. Чтобы указать значение sourceAnchor для данного локального объекта AD, настройте его атрибут msDS-ConsistencyGuid перед его импортом в Azure AD Подключение. 
  
Дополнительные сведения о SourceAnchor и ConsistencyGuid можно найти в следующих сведениях: [Azure AD Подключение: концепции проектирования](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

