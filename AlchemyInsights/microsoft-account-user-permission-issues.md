---
title: Проблема устранения неполадок . Пользователь, не найденный в каталоге
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098183"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Проблема устранения неполадок . Пользователь, не найденный в каталоге

Если пользователи получают сообщение об ошибке "пользователь не может быть найден" в каталоге, попробуйте еще раз, где тип проблемы — пользователь, не в каталоге.

Для устранения неполадок можно завершить следующие действия.

- Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для регистрации позже. Убедитесь, что пользователь использует ту же учетную запись, чтобы принять приглашение и войти на сайт. 

Дополнительные сведения см. [в журнале How to manage aliases for your Microsoft account </a> to manage the Microsoft 365 входа.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Просмотрите каждый сайт(ы), на котором пользователь получает ошибку. 

Добавьте "/_layouts/15/people.aspx/membershipgroupid=0" (в двух кавычках) в конце URL-адреса сайта. 

Пример: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Выберите пользователя из списка.

- Щелкните **Удалить разрешения пользователей** из ленты. 
-  Добавьте обратно пользователя и resend приглашение к пользователю.

