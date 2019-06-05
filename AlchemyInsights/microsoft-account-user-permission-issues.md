---
title: Создание и использование общего почтового ящика
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717359"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Устранение неполадок — пользователь не найден в каталоге

<p>Если пользователи получают сообщение об ошибке, <strong> &ldquo; &hellip;в каталоге можно&rsquo;найти пользователя с сообщением об ошибке. Повторите попытку&hellip; </strong> , где тип проблемы — " <strong> &ldquo;пользователь не находится в&rdquo;каталоге".</strong>чтобы устранить эту проблему, можно выполнить следующие действия.</p> <ol> <li>Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже. Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт. <br /><br />Для получения дополнительных сведений Узнайте, <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">как управлять псевдонимами для учетной записи Майкрософт</a> для управления учетными данными Office 365. <br /><br /></li> <li>Перейдите на каждый сайт, где пользователь получает сообщение об ошибке. <br /><br />а. Добавьте <strong> &ldquo;/_layouts/15/People.aspx/membershipgroupid = 0&rdquo; </strong> (в двойных кавычках) до конца URL-адреса сайта. <br /><br />Пример: https://&lt;contoso&gt;. SharePoint.com/_layouts/15/People.aspx/membershipGroupId=0 <br /><br />б) Выберите пользователя в списке. <br /><br />В. Нажмите кнопку <strong>удалить разрешения пользователя на ленте</strong>. <br /><br />Г. Добавить пользователя и повторно отправить приглашение для пользователя.</li> </ol>

