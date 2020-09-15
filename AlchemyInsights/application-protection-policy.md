---
title: Политика защиты приложений
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716906"
---
# <a name="application-protection-policy"></a><span data-ttu-id="a04e8-102">Политика защиты приложений</span><span class="sxs-lookup"><span data-stu-id="a04e8-102">Application protection policy</span></span>

<span data-ttu-id="a04e8-103">Если вы еще не работали с политикой защиты приложений (APP), см. статью [Обзор политик защиты приложений](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="a04e8-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="a04e8-104">Прежде чем приступить к работе с политиками защиты приложений, см. статью [Как создавать и назначать политики защиты приложений](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="a04e8-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="a04e8-105">Требования к политике защиты приложений:</span><span class="sxs-lookup"><span data-stu-id="a04e8-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="a04e8-106">У пользователя есть лицензия Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="a04e8-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="a04e8-107">Пользователь входит в группу, для которой предназначены политики защиты приложений.</span><span class="sxs-lookup"><span data-stu-id="a04e8-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="a04e8-108">Только один корпоративный пользователь выполнил вход в защищенные приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a04e8-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="a04e8-109">Приложение реализовало пакет [SDK Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="a04e8-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="a04e8-110">Список приложений, поддерживающих пакет SDK, см. в статье [Приложения, защищенные Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="a04e8-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="a04e8-111">Политики применяются после того, как пользователь, отвечающий приведенным выше требованиям, выполнит вход в приложение, поддерживающее пакет SDK Intune.</span><span class="sxs-lookup"><span data-stu-id="a04e8-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="a04e8-112">Самый простой способ определить, применяется ли политика, — это потребовать, чтобы пользователь задал в политике ПИН-код.</span><span class="sxs-lookup"><span data-stu-id="a04e8-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="a04e8-113">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="a04e8-113">For more information, see:</span></span>

[<span data-ttu-id="a04e8-114">Вопросы и ответы по устранению неполадок APP/MAM</span><span class="sxs-lookup"><span data-stu-id="a04e8-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="a04e8-115">Способ проверки настроек политики защиты приложений</span><span class="sxs-lookup"><span data-stu-id="a04e8-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="a04e8-116">Общие сведения о времени доставки политики защиты приложений</span><span class="sxs-lookup"><span data-stu-id="a04e8-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="a04e8-117">Как отслеживать политики защиты приложений</span><span class="sxs-lookup"><span data-stu-id="a04e8-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)