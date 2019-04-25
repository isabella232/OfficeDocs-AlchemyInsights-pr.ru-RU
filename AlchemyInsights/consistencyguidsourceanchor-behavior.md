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
# <a name="consistencyguid--sourceanchor-behavior"></a>Поведение Консистенцигуид и Саурцеанчор

Azure AD Connect (версии 1.1.524.0 и After) теперь способствует использованию атрибута msDS-Консистенцигуид в качестве атрибута Саурцеанчор. При использовании этой функции служба Azure AD Connect автоматически настраивает правила синхронизации следующим образом:
  
- Используйте msDS — Консистенцигуид в качестве атрибута Саурцеанчор для объектов User. ObjectGUID используется для других типов объектов.
    
- Для любого объекта локального пользователя AD, чей атрибут msDS — Консистенцигуид не заполнен, Azure AD Connect записывает значение objectGUID обратно в атрибут msDS – Консистенцигуид в локальной службе Active Directory. После заполнения атрибута msDS-Консистенцигуид Azure AD Connect затем экспортирует объект в Azure AD.
    
 **Примечание:** После того как локальный объект AD импортируется в Azure AD Connect (то есть импортируется в пространство AD Connector и проецируется в метавселенной), его значение Саурцеанчор больше нельзя изменить. Чтобы указать значение Саурцеанчор для данного локального объекта AD, настройте его атрибут msDS-Консистенцигуид перед его импортом в Azure AD Connect. 
  
Дополнительные сведения о Саурцеанчор и Консистенцигуид можно найти в следующих статьях: [Azure AD Connect: концепции дизайна](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

