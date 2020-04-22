---
title: Устранение неполадок — пользователь не найден в каталоге
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702751"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Устранение неполадок — пользователь не найден в каталоге

Если пользователи получают сообщение об ошибке "пользователь не может быть найден" в каталоге, повторите попытку, где тип вопроса — "пользователь не находится в каталоге".

Чтобы устранить эту проблему, можно выполнить следующие действия.

- Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже. Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт. 

Дополнительные сведения о том, [как управлять псевдонимами для учетной записи</a> Майкрософт для управления учетной записью Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Перейдите на каждый сайт, где пользователь получает сообщение об ошибке. 

Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта. 

Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Выберите пользователя в списке.

- Нажмите кнопку **удалить разрешения пользователя** на ленте. 
-  Добавить пользователя и повторно отправить приглашение для пользователя.

