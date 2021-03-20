---
title: Настройка сквозной проверки подлинности через Azure Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898176"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="cbd86-102">Настройка сквозной проверки подлинности через Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cbd86-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="cbd86-103">Вот некоторые руководства по настройке сквозной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cbd86-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="cbd86-104">**Настройка Azure Active Directory Connect**. Руководство [Синхронизация пользователей с каталогом](https://admin.microsoft.com/AdminPortal/Home) поможет настроить синхронизацию хэша паролей или сквозную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="cbd86-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="cbd86-105">Эта конфигурация позволяет пользователям входить в свою электронную почту и в локальную службу Active Directory (контроллер домена), используя один и тот же пароль.</span><span class="sxs-lookup"><span data-stu-id="cbd86-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="cbd86-106">В руководстве [Синхронизация пользователей с каталогом](https://admin.microsoft.com/AdminPortal/Home) также описывается вход в федерацию с использованием служб федерации Active Directory (AD FS).</span><span class="sxs-lookup"><span data-stu-id="cbd86-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="cbd86-107">**Настройка функций Azure**. В [Руководстве по настройке Azure AD](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) детально описывается процесс настройки функций в Azure Active Directory Basic, таких как управление доступом на основе групп, самостоятельный сброс пароля для облачных приложений и прокси-сервер приложений Azure Active Directory для публикации локальных веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="cbd86-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


