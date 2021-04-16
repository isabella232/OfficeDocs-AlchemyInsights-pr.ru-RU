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
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813773"
---
# <a name="error-attributevaluemustbeunique"></a>Ошибка: AttributeValueMustBeUnique

Наиболее распространенной причиной ошибки AttributeValueMustBeUnique является то, что два объекта с разными свойствами SourceAnchor (immutableId) имеют одинаковое значение для атрибутов ProxyAddresses и/или UserPrincipalName. Чтобы исправить ошибку AttributeValueMustBeUnique:
  
1. Определите дублированные прокси-серверы, userPrincipalName или другое значение атрибута, из-за чего произошла ошибка. Также определите, какие два (или более) объекта вовлечены в конфликт. Отчет azure AD Connect Health для синхронизации поможет определить два объекта.
    
2. Определите, какой объект должен по-прежнему иметь дублирующее значение, а какой объект не должен.
    
3. Удалите дублирующее значение из объекта, которое не должно иметь этого значения. Обратите внимание, что необходимо внести изменения в каталог, в котором объект был источником. В некоторых случаях может потребоваться удалить один из конфликтуемых объектов.
    
4. Если вы в изменились в локальной AD, пусть Azure AD Connect синхронизирует изменение, чтобы ошибка была исправлена.
    

