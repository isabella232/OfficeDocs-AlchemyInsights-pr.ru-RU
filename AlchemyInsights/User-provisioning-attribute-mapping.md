---
title: Сопоставление атрибутов подготовки пользователей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935395"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="090d4-102">Сопоставление атрибутов подготовки пользователей</span><span class="sxs-lookup"><span data-stu-id="090d4-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="090d4-103">Чтобы устранить известные проблемы при сопоставлении атрибутов, см. статью [Сопоставления атрибутов](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="090d4-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="090d4-104">Microsoft Azure Active Directory (AD) обеспечивает поддержку подготовки пользователей для сторонних приложений SaaS, таких как Salesforce, G Suite и др.</span><span class="sxs-lookup"><span data-stu-id="090d4-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="090d4-105">Если включена подготовка пользователей для стороннего приложения SaaS, портал Azure управляет значениями его атрибутов с помощью сопоставлений атрибутов.</span><span class="sxs-lookup"><span data-stu-id="090d4-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="090d4-106">Сведения о настройке сопоставлений атрибутов по умолчанию см. в статье [Настройка сопоставлений атрибутов подготовки пользователей для приложений SaaS в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="090d4-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="090d4-107">Дополнительные сведения о подготовке пользователей приложения SaaS см. в статье [Что такое автоматизированная подготовка пользователей приложения SaaS в Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="090d4-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="090d4-108">При настройке сопоставлений атрибутов для подготовки пользователей может оказаться, что атрибут, который нужно сопоставить, не отображается в списке атрибутов источника.</span><span class="sxs-lookup"><span data-stu-id="090d4-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="090d4-109">В статье [Синхронизация атрибута из локальной службы Active Directory с Azure AD для подготовки приложения](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) показано, как добавлять отсутствующий атрибут, выполняя его синхронизацию из локальной службы AD с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="090d4-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
