---
title: Сведения об удостоверениях в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664183"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="ae00a-102">Сведения об удостоверениях в Yammer</span><span class="sxs-lookup"><span data-stu-id="ae00a-102">About identity in Yammer</span></span>

<span data-ttu-id="ae00a-103">Чтобы избежать проблем, связанных с удостоверениями, рекомендуется выполнить перечисленные ниже действия во всех сетях.</span><span class="sxs-lookup"><span data-stu-id="ae00a-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="ae00a-104">Используйте удостоверение Office 365 после подготовки учетных записей Microsoft 365 для пользователей в Azure AD, чтобы все пользователи могли входить в систему с помощью своей основной учетной записи Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ae00a-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="ae00a-105">Дополнительные сведения см. в статье [Использование удостоверения Office 365 для Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="ae00a-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="ae00a-106">Объединение нескольких сетей Yammer.</span><span class="sxs-lookup"><span data-stu-id="ae00a-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="ae00a-107">Устаревшие конфигурации Yammer позволяют подключаться к нескольким сетям Yammer с одним клиентом.</span><span class="sxs-lookup"><span data-stu-id="ae00a-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="ae00a-108">Дополнительные сведения см. в статье [Сетевая миграция: объединение нескольких сетей Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="ae00a-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="ae00a-109">Можно также применять лицензирование Yammer для блокировки пользователей из Yammer, если у них нет лицензии.</span><span class="sxs-lookup"><span data-stu-id="ae00a-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="ae00a-110">Дополнительные сведения см. в статье [Управление лицензиями пользователей Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="ae00a-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="ae00a-111">Наконец, проведите аудит списка пользователей для старых сетей Yammer и отключите прежних пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae00a-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="ae00a-112">Рекомендуется отключить (деактивировать) пользователей, не удаляя их, потому что удаление необратимо.</span><span class="sxs-lookup"><span data-stu-id="ae00a-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="ae00a-113">Дополнительные сведения см. в статьях [Аудит пользователей Yammer в сетях, подключенных к Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) и [Удаление пользователей](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="ae00a-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="ae00a-114">С помощью этих действий можно также настроить сеть Yammer для основного режима в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ae00a-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="ae00a-115">Дополнительные сведения см. в статье [Настройка сети Yammer для основного режима в Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="ae00a-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>