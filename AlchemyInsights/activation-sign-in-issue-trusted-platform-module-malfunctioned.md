---
title: Проблема активации и входов — сбой в работе доверенного модуля платформы
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822900"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0f71c-102">Исправление приложения Microsoft 365 "Модуль доверенных платформ компьютера не функционирует должным образом" сообщение</span><span class="sxs-lookup"><span data-stu-id="0f71c-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0f71c-103">Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0f71c-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="0f71c-104">Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="0f71c-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="0f71c-105">С помощью  >  **учетных записей параметров** Windows  >  **& учетные записи,** удалите существующие учетные записи.</span><span class="sxs-lookup"><span data-stu-id="0f71c-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove existing work accounts.</span></span> 
3. <span data-ttu-id="0f71c-106">С помощью windows **Settings**  >  **Accounts**  >  **Access work or school** отключите существующие учетные записи.</span><span class="sxs-lookup"><span data-stu-id="0f71c-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect existing accounts.</span></span> 
4. <span data-ttu-id="0f71c-107">Сбросьте состояние активации Office.</span><span class="sxs-lookup"><span data-stu-id="0f71c-107">Reset Office activation state.</span></span> <span data-ttu-id="0f71c-108">[Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)</span><span class="sxs-lookup"><span data-stu-id="0f71c-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="0f71c-109">Попробуйте [процесс восстановления пользователей,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) чтобы устранить сбои в работе модуля доверенных платформ (TPM).</span><span class="sxs-lookup"><span data-stu-id="0f71c-109">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>