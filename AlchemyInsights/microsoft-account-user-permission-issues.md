---
title: Устранение неполадок — пользователь не найден в каталоге
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725420"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Устранение неполадок — пользователь не найден в каталоге

Если пользователи получают сообщение об ошибке "пользователь не может быть найден" в каталоге, повторите попытку, где тип вопроса — "пользователь не находится в каталоге".

Чтобы устранить эту проблему, можно выполнить следующие действия.

- Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже. Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт. 

Дополнительные сведения о том, [как управлять псевдонимами для учетной записи Майкрософт для управления учетной записью </a> Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Перейдите на каждый сайт, где пользователь получает сообщение об ошибке. 

Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта. 

Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Выберите пользователя в списке.

- Нажмите кнопку **удалить разрешения пользователя** на ленте. 
-  Добавить пользователя и повторно отправить приглашение для пользователя.

