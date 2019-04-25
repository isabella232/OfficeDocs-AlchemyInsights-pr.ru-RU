---
title: Условный доступ с помощью Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393554"
---
# <a name="conditional-access-with-intune"></a>Условный доступ с помощью Intune

Для использования **условНого доступа** в Intune необходимо 3 этапа: 
  
- Создайте **политику условНого доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам. Например, устройство должно быть совместимо перед доступом к корпоративной почте. 
    
- Создайте **политику соответствия требованиям** , чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым. Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым. 
    
- Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory. 
    
Дополнительные сведения:
  
- [Рекомендации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Начало работы с условным доступом](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

