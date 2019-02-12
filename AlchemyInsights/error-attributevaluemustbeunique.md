---
title: Ошибка AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916537"
---
# <a name="error-attributevaluemustbeunique"></a>Ошибка: AttributeValueMustBeUnique

Наиболее распространенные причины возникновения ошибки AttributeValueMustBeUnique является два объекта с другой SourceAnchor (immutableId) с таким же значением для атрибутов ProxyAddresses и/или UserPrincipalName. Чтобы устранить ошибку AttributeValueMustBeUnique:
  
1. Определение повторяющихся proxyAddresses, userPrincipalName или другие значения атрибута, который вызывает ошибку. Также определите, какие объекты двух (или более) участвуют в конфликт. Созданный Azure AD подключение работоспособности для синхронизации может помочь определить два объекта.
    
2. Определите, какой объект должны продолжать повторяющиеся значения и какой объект не должен.
    
3. Удалите повторяющиеся значения из объекта, который не должно быть это значение. Обратите внимание на то, что необходимо внести изменения в каталог, где объект привязывается из. В некоторых случаях может потребоваться удалить одного из объектов в конфликта.
    
4. Если вы внесли изменения в локальный AD, позволяют Azure AD подключить синхронизировать изменение текста Error для устранения.
    

