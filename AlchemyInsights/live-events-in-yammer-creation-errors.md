---
title: Ошибки при создании трансляций в Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675455"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="96937-102">Ошибки при создании трансляций в Yammer</span><span class="sxs-lookup"><span data-stu-id="96937-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="96937-103">**Создание трансляций Yammer**</span><span class="sxs-lookup"><span data-stu-id="96937-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="96937-104">В Yammer будет отображаться параметр, позволяющий создать трансляцию в любое время.</span><span class="sxs-lookup"><span data-stu-id="96937-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="96937-105">В некоторых случаях пользователь может не соответствовать предварительным требованиям для создания трансляции. Тогда при попытке создания может возникнуть ошибка.</span><span class="sxs-lookup"><span data-stu-id="96937-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="96937-106">В приведенных ниже разделах рассматриваются распространенные причины этой проблемы и способы ее устранения для пользователей.</span><span class="sxs-lookup"><span data-stu-id="96937-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="96937-107">**Кто может создавать трансляции**</span><span class="sxs-lookup"><span data-stu-id="96937-107">**Who can create live events**</span></span>
- <span data-ttu-id="96937-108">Лицензия Office 365 корпоративный E1, E3 или E5 либо Office 365 A3 или A5.</span><span class="sxs-lookup"><span data-stu-id="96937-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="96937-109">Разрешение на создание трансляций в Центре администрирования Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="96937-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="96937-110">Разрешение на создание трансляций в Microsoft Stream (для трансляций, создаваемых с использованием внешнего вещательного приложения или устройства).</span><span class="sxs-lookup"><span data-stu-id="96937-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="96937-111">Полное членство в команде организации (не может быть гостем или из другой организации).</span><span class="sxs-lookup"><span data-stu-id="96937-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="96937-112">Планирование частных собраний, демонстрация экрана и общий доступ к IP-видео включены в политике собраний команды.</span><span class="sxs-lookup"><span data-stu-id="96937-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="96937-113">**Политики создания трансляций**</span><span class="sxs-lookup"><span data-stu-id="96937-113">**Live event creation policies**</span></span>

<span data-ttu-id="96937-114">Yammer следует политикам трансляций, установленным в клиенте Office 365 для Stream.</span><span class="sxs-lookup"><span data-stu-id="96937-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="96937-115">По умолчанию любой пользователь в организации может создать трансляцию.</span><span class="sxs-lookup"><span data-stu-id="96937-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="96937-116">Администраторы могут [вносить изменения в этот параметр, чтобы запретить пользователям создание трансляции](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="96937-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="96937-117">Если возникает ошибка политики, важно убедиться в том, что у пользователей есть разрешения на создание трансляций.</span><span class="sxs-lookup"><span data-stu-id="96937-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
