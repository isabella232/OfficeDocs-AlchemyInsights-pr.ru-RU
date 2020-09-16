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
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f3658-102">Устранение неполадок — пользователь не найден в каталоге</span><span class="sxs-lookup"><span data-stu-id="f3658-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f3658-103">Если пользователи получают сообщение об ошибке "пользователь не может быть найден" в каталоге, повторите попытку, где тип вопроса — "пользователь не находится в каталоге".</span><span class="sxs-lookup"><span data-stu-id="f3658-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f3658-104">Чтобы устранить эту проблему, можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="f3658-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f3658-105">Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже.</span><span class="sxs-lookup"><span data-stu-id="f3658-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f3658-106">Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт.</span><span class="sxs-lookup"><span data-stu-id="f3658-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f3658-107">Дополнительные сведения о том, [как управлять псевдонимами для учетной записи Майкрософт для управления учетной записью </a> Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f3658-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f3658-108">Перейдите на каждый сайт, где пользователь получает сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f3658-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f3658-109">Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта.</span><span class="sxs-lookup"><span data-stu-id="f3658-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f3658-110">Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f3658-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f3658-111">Выберите пользователя в списке.</span><span class="sxs-lookup"><span data-stu-id="f3658-111">Select the user from the list.</span></span>

- <span data-ttu-id="f3658-112">Нажмите кнопку **удалить разрешения пользователя** на ленте.</span><span class="sxs-lookup"><span data-stu-id="f3658-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f3658-113">Добавить пользователя и повторно отправить приглашение для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f3658-113">Add back the User and Resend the invite to the user.</span></span>

