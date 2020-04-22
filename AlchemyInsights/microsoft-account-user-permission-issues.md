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
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="46e13-102">Устранение неполадок — пользователь не найден в каталоге</span><span class="sxs-lookup"><span data-stu-id="46e13-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="46e13-103">Если пользователи получают сообщение об ошибке "пользователь не может быть найден" в каталоге, повторите попытку, где тип вопроса — "пользователь не находится в каталоге".</span><span class="sxs-lookup"><span data-stu-id="46e13-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="46e13-104">Чтобы устранить эту проблему, можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="46e13-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="46e13-105">Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже.</span><span class="sxs-lookup"><span data-stu-id="46e13-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="46e13-106">Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт.</span><span class="sxs-lookup"><span data-stu-id="46e13-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="46e13-107">Дополнительные сведения о том, [как управлять псевдонимами для учетной записи</a> Майкрософт для управления учетной записью Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="46e13-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="46e13-108">Перейдите на каждый сайт, где пользователь получает сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="46e13-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="46e13-109">Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта.</span><span class="sxs-lookup"><span data-stu-id="46e13-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="46e13-110">Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="46e13-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="46e13-111">Выберите пользователя в списке.</span><span class="sxs-lookup"><span data-stu-id="46e13-111">Select the user from the list.</span></span>

- <span data-ttu-id="46e13-112">Нажмите кнопку **удалить разрешения пользователя** на ленте.</span><span class="sxs-lookup"><span data-stu-id="46e13-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="46e13-113">Добавить пользователя и повторно отправить приглашение для пользователя.</span><span class="sxs-lookup"><span data-stu-id="46e13-113">Add back the User and Resend the invite to the user.</span></span>

