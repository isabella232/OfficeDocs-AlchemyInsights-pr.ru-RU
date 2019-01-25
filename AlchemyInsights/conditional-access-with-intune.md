---
title: Условное доступа с Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486792"
---
# <a name="conditional-access-with-intune"></a>Условное доступа с Intune

Использование **Условного доступа** с Intune требуется три этапа: 
  
- Создайте **Условную политику доступа** , который определяет, какие ресурсы защищены и условия, необходимые для быть выполнены для доступа к ресурсам. Например устройства должны быть совместимыми перед доступом к корпоративной электронной почты. 
    
- Создание **Политики соответствия** для определения параметров, которые должны быть выполнены перед считается совместимые устройства. Например устройство ПИН-кодов по крайней мере 6 цифр перед необходимо считается спецификации. 
    
- Настройка **Политики соответствия** и **Условной политики доступа** предназначены для нужного групп пользователей. Может потребоваться создание определенных групп пользователей в Azure Active Directory. 
    
Дополнительные сведения
  
- [Рекомендации по условного доступа](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [Приступая к работе с условным доступом](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

