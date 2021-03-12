---
title: Политики паролей
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718206"
---
# <a name="password-policies"></a><span data-ttu-id="14856-102">Политики паролей</span><span class="sxs-lookup"><span data-stu-id="14856-102">Password policies</span></span>

<span data-ttu-id="14856-103">**У меня возникли проблемы с политикой паролей для пользователя**</span><span class="sxs-lookup"><span data-stu-id="14856-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="14856-104">Политика паролей для пользователя зависит от того, является ли пользователь облачным или локально.</span><span class="sxs-lookup"><span data-stu-id="14856-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="14856-105">Только пользователи облака должны выбрать пароль, отвечающий требованиям в этой статье: политики паролей, применимые только [к облачным учетным записям пользователей.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="14856-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="14856-106">Локальному пользователю необходимо выбрать пароль, отвечающий требованиям локального доступа.</span><span class="sxs-lookup"><span data-stu-id="14856-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="14856-107">Если локальному пользователю не удается установить пароль, проверьте свои требования к локальной сети.</span><span class="sxs-lookup"><span data-stu-id="14856-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="14856-108">**Я не знаю, как установить или проверить политики истечения срока действия пароля**</span><span class="sxs-lookup"><span data-stu-id="14856-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="14856-109">Вы можете установить и проверить политику истечения срока действия для пользователей облака в клиенте с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14856-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="14856-110">Следуйте инструкциям в этой статье: Установите или проверьте политики паролей [с помощью PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="14856-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="14856-111">Политика истечения срока действия пароля для локального пользователя задается в локальной AD.</span><span class="sxs-lookup"><span data-stu-id="14856-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="14856-112">**Другие полезные ссылки:**</span><span class="sxs-lookup"><span data-stu-id="14856-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="14856-113">Начало работы с сбросом пароля</span><span class="sxs-lookup"><span data-stu-id="14856-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="14856-114">Устранение неполадок с инициированным администратором сбросом пароля</span><span class="sxs-lookup"><span data-stu-id="14856-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
