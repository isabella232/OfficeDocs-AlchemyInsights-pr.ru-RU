---
title: Условный доступ с помощью Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706034"
---
# <a name="conditional-access-with-intune"></a>Условный доступ с помощью Intune

Для использования **условного доступа** в Intune необходимо 3 этапа: 
  
- Создайте **политику условного доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам. Например, устройство должно быть совместимо перед доступом к корпоративной почте. 
    
- Создайте **политику соответствия требованиям** , чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым. Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым. 
    
- Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory. 
    
Дополнительные сведения:
  
- [Рекомендации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Начало работы с условным доступом](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

