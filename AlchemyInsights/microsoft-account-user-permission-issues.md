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
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762413"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ef3c1-102">Устранение неполадок — пользователь не найден в каталоге</span><span class="sxs-lookup"><span data-stu-id="ef3c1-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ef3c1-103">Если пользователи получают сообщение об ошибке "не удается найти пользователя" в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ef3c1-104">Повторите попытку, где тип вопроса — "пользователь не находится в каталоге".</span><span class="sxs-lookup"><span data-stu-id="ef3c1-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ef3c1-105">Чтобы устранить эту проблему, можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ef3c1-106">Убедитесь, что учетная запись, которая приняла приглашение электронной почты, является той же учетной записью, которая используется для входа в систему позже.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ef3c1-107">Убедитесь, что пользователь использует одну и ту же учетную запись для принятия приглашения и входа на сайт.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ef3c1-108">Для получения дополнительных сведений Узнайте, [как управлять псевдонимами для учетной</a> записи Майкрософт для управления учетными данными Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ef3c1-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ef3c1-109">Перейдите на каждый сайт, где пользователь получает сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ef3c1-110">Добавьте "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойных кавычках) до конца URL-адреса сайта.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ef3c1-111">Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ef3c1-112">Выберите пользователя в списке.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-112">Select the user from the list.</span></span>

- <span data-ttu-id="ef3c1-113">Нажмите кнопку **удалить разрешения пользователя** на ленте.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ef3c1-114">Добавить пользователя и повторно отправить приглашение для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef3c1-114">Add back the User and Resend the invite to the user.</span></span>

