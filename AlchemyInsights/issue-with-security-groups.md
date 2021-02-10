---
title: Проблема с группами безопасности
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162946"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="cb470-102">Проблема с группами безопасности</span><span class="sxs-lookup"><span data-stu-id="cb470-102">Issue with security groups</span></span>

<span data-ttu-id="cb470-103">**Если отображается сообщение об ошибке сети AADDS104**</span><span class="sxs-lookup"><span data-stu-id="cb470-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="cb470-104">Недопустимые правила группы безопасности сети являются наиболее частой причиной сетевых ошибок для доменных служб Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="cb470-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="cb470-105">Группа безопасности для виртуальной сети должна разрешать доступ к определенным портам и протоколам.</span><span class="sxs-lookup"><span data-stu-id="cb470-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="cb470-106">Если такие порты заблокированы, платформа Azure не сможет отслеживать или обновлять управляемые домены.</span><span class="sxs-lookup"><span data-stu-id="cb470-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="cb470-107">Это также влияет на синхронизацию между службами Azure AD и Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="cb470-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="cb470-108">Убедитесь, что порты по умолчанию открыты, чтобы избежать перерывов в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="cb470-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="cb470-109">Сведения об устранении распространенных оповещений о проблемах, связанных с настройкой группы безопасности сети, см. в статье [Добавление и проверка групп безопасности](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="cb470-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
