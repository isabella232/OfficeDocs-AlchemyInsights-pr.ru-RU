---
title: Надстройка Teams для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617116"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="a76e3-102">Надстройка Teams для Mac</span><span class="sxs-lookup"><span data-stu-id="a76e3-102">Teams add-in for Mac</span></span>

<span data-ttu-id="a76e3-103">Чтобы устранить проблему с отсутствующей надстройкой Teams для пользователей операционной системы компьютеров Mac, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="a76e3-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="a76e3-104">**Шаг 1.** При локальном применении гибридной среды Exchange (версия 2016 с накопительным пакетом обновления 3 или более поздняя версия) используйте средство Test-HMA.ps1, чтобы подтвердить правильность настройки гибридной современной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a76e3-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="a76e3-105">Дополнительные сведения см. в разделе [Проверка настройки гибридной современной проверки подлинности в Outlook для iOS и Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="a76e3-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="a76e3-106">**Примечание**. Используйте формат адреса UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)), а не домен\имя_пользователя.</span><span class="sxs-lookup"><span data-stu-id="a76e3-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="a76e3-107">Выполняйте это даже для пользователей с почтовыми ящиками Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a76e3-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="a76e3-108">**Шаг 2.** Попросите пользователя перейти в раздел **Средства** > **Учетные записи**... в Outlook для Mac, а затем найти и выбрать учетную запись.</span><span class="sxs-lookup"><span data-stu-id="a76e3-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="a76e3-109">Убедитесь, что имя пользователя указано в формате UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="a76e3-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="a76e3-110">**Шаг 3.** Подтвердите, что пользователь является лицензированным пользователем Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a76e3-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="a76e3-111">Пользователь должен использовать подписку на Office 365 для Mac версии 16.24 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="a76e3-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>