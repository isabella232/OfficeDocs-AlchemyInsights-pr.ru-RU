---
title: Развертывание Microsoft Edge в iOS, iPadOS и Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178002"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="619e9-102">Развертывание Microsoft Edge в iOS, iPadOS и Android</span><span class="sxs-lookup"><span data-stu-id="619e9-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="619e9-103">Описанный ниже интерактивный сценарий поможет назначить Microsoft Edge пользователям устройств с iOS, iPadOS и Android.</span><span class="sxs-lookup"><span data-stu-id="619e9-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="619e9-104">Ели вы запретите пользователям регистрировать мобильные устройства, этот интерактивный сценарий не будет работать и им придется установить Microsoft Edge самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="619e9-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="619e9-105">Этот интерактивный сценарий включает следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="619e9-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="619e9-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="619e9-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="619e9-107">Введение</span><span class="sxs-lookup"><span data-stu-id="619e9-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="619e9-108">Основы</span><span class="sxs-lookup"><span data-stu-id="619e9-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="619e9-109">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="619e9-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="619e9-110">Задания</span><span class="sxs-lookup"><span data-stu-id="619e9-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="619e9-111">Проверка и создание</span><span class="sxs-lookup"><span data-stu-id="619e9-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="619e9-112">Когда шаги из интерактивного сценария будут выполнены, политики Microsoft Intune включат следующие возможности Microsoft Edge для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="619e9-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="619e9-113">Двойное удостоверение</span><span class="sxs-lookup"><span data-stu-id="619e9-113">Dual identity</span></span>
- <span data-ttu-id="619e9-114">Интеграция с политикой защиты приложений Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="619e9-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="619e9-115">Интеграция с Azure Active Directory Application Proxy</span><span class="sxs-lookup"><span data-stu-id="619e9-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="619e9-116">Управляемое избранное и ярлыки домашней страницы</span><span class="sxs-lookup"><span data-stu-id="619e9-116">Managed favorites and home page shortcuts</span></span>
