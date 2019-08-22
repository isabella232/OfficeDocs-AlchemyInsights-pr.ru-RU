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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505007"
---
# <a name="conditional-access-with-intune"></a>Условный доступ с помощью Intune

Для использования **условного доступа** в Intune необходимо 3 этапа: 
  
- Создайте **политику условного доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам. Например, устройство должно быть совместимо перед доступом к корпоративной почте. 
    
- Создайте **политику соответствия требованиям** , чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым. Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым. 
    
- Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory. 
    
Дополнительные сведения:
  
- [Рекомендации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Начало работы с условным доступом](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

