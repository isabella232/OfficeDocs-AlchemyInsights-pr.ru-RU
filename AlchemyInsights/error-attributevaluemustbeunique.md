---
title: Ошибка Аттрибутевалуемустбеуникуе
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709164"
---
# <a name="error-attributevaluemustbeunique"></a>Ошибка: Аттрибутевалуемустбеуникуе

Наиболее распространенная причина ошибки Аттрибутевалуемустбеуникуе — два объекта с разными Саурцеанчор (значения свойств ImmutableId) имеют одинаковое значение для атрибутов ProxyAddresses и/или UserPrincipalName. Чтобы исправить ошибку Аттрибутевалуемустбеуникуе, выполните указанные ниже действия.
  
1. Определите дубликат proxyAddresses, userPrincipalName или другое значение атрибута, которое вызывает ошибку. Кроме того, определите, какие два (или более) объекта участвуют в конфликте. Отчет, созданный с помощью Azure AD Connect Health для синхронизации, поможет вам определить два объекта.
    
2. Определите, в каком объекте должно продолжаться дублированное значение, а какие нет.
    
3. Удалите повторяющееся значение из объекта, который не должен иметь это значение. Обратите внимание, что необходимо внести изменения в каталог, из которого источник объекта. В некоторых случаях может потребоваться удалить один из объектов в конфликте.
    
4. Если вы внесли изменения в локальное AD, позвольте Azure AD Connect синхронизировать изменения, чтобы исправить ошибку, чтобы исправить ошибку.
    

