---
title: Развертывание Microsoft Edge для мобильных устройств для iOS, iPadOS или Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652236"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="c305d-102">Развертывание Microsoft Edge для мобильных устройств для iOS, iPadOS или Android</span><span class="sxs-lookup"><span data-stu-id="c305d-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="c305d-103">С помощью приведенного ниже сценария вы сможете назначить Microsoft Edge пользователям устройств с iOS, iPadOS и Android.</span><span class="sxs-lookup"><span data-stu-id="c305d-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="c305d-104">После выполнения этих действий политики Microsoft Intune встроят следующие функции Microsoft Edge для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="c305d-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="c305d-105">Двойное удостоверение</span><span class="sxs-lookup"><span data-stu-id="c305d-105">Dual identity</span></span>
- <span data-ttu-id="c305d-106">Интеграция с политикой защиты приложений Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c305d-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="c305d-107">Интеграция с прокси приложения Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c305d-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="c305d-108">Управляемые избранное и ярлыки домашней страницы</span><span class="sxs-lookup"><span data-stu-id="c305d-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="c305d-109">Если вы заблокировали для пользователей регистрацию мобильных устройств, этот сценарий не будет работать, и пользователям потребуется установить Microsoft Edge самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="c305d-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="c305d-110">Чтобы развернуть Microsoft Edge для мобильных устройств для iOS, iPadOS или Android, см.:</span><span class="sxs-lookup"><span data-stu-id="c305d-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="c305d-111">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c305d-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="c305d-112">Введение</span><span class="sxs-lookup"><span data-stu-id="c305d-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="c305d-113">Основы</span><span class="sxs-lookup"><span data-stu-id="c305d-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="c305d-114">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="c305d-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. <span data-ttu-id="c305d-115">[назначения](https://go.microsoft.com/fwlink/?linkid=2132869);</span><span class="sxs-lookup"><span data-stu-id="c305d-115">[Assignments](https://go.microsoft.com/fwlink/?linkid=2132869)</span></span>
6. [<span data-ttu-id="c305d-116">Просмотр и создание</span><span class="sxs-lookup"><span data-stu-id="c305d-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
