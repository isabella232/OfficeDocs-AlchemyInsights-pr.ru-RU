---
title: Ошибка AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002133"
---
# <a name="error-attributevaluemustbeunique"></a>Ошибка: AttributeValueMustBeUnique

Наиболее распространенной причиной ошибки AttributeValueMustBeUnique является то, что два объекта с разными свойствами SourceAnchor (immutableId) имеют одинаковое значение для атрибутов ProxyAddresses и/или UserPrincipalName. Чтобы исправить ошибку AttributeValueMustBeUnique:
  
1. Определите дублированные прокси-серверы, userPrincipalName или другое значение атрибута, из-за чего произошла ошибка. Также определите, какие два (или более) объекта вовлечены в конфликт. Отчет, созданный службой Azure AD Подключение для синхронизации, поможет определить два объекта.
    
2. Определите, какой объект должен по-прежнему иметь дублирующее значение, а какой объект не должен.
    
3. Удалите дублирующее значение из объекта, которое не должно иметь этого значения. Обратите внимание, что необходимо внести изменения в каталог, в котором объект был источником. В некоторых случаях может потребоваться удалить один из конфликтуемых объектов.
    
4. Если вы в изменились в локальной AD, Подключение Azure AD синхронизируйте изменение для исправлений ошибки.
    

