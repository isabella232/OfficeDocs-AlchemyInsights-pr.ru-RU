---
title: Устранение неполадок — пользователь не найден в каталоге
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249926"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Устранение неполадок — пользователь не найден в каталоге

Если пользователи получают сообщение об ошибке "не удается найти пользователя" в каталоге. Повторите попытку, где тип вопроса — "пользователь не находится в каталоге".

Чтобы устранить эту проблему, можно выполнить следующие действия.

- Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже. Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт. 

Для получения дополнительных сведений Узнайте, [как управлять псевдонимами для учетной</a> записи Майкрософт для управления учетными данными Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Перейдите на каждый сайт, где пользователь получает сообщение об ошибке. 

Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта. 

Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Выберите пользователя в списке.

- Нажмите кнопку **удалить разрешения пользователя** на ленте. 
-  Добавить пользователя и повторно отправить приглашение для пользователя.

