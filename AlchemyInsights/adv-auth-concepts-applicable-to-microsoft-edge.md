---
title: Дополнительные понятия проверки подлинности, применяемые к Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571892"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="35e8d-102">Дополнительные понятия проверки подлинности, применяемые к Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="35e8d-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="35e8d-103">Ниже приведены основные концепции проверки подлинности, которые относятся к Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="35e8d-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="35e8d-104">**Упреждающий способ проверки подлинности**</span><span class="sxs-lookup"><span data-stu-id="35e8d-104">**Proactive Authentication**</span></span>

<span data-ttu-id="35e8d-105">При включении политики [Проактивеаусенаблед](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge будет пытаться выполнять проверку подлинности пользователей, вошедших в систему, с помощью служб Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35e8d-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="35e8d-106">Через заданные промежутки времени она будет использовать веб-службу для проверки обновленного манифеста, содержащего конфигурацию для профилактической проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="35e8d-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="35e8d-107">Преимущества: упреждающее аутентификация обеспечивает проверку подлинности для ключевых служб, таких как страница новой вкладки Office.</span><span class="sxs-lookup"><span data-stu-id="35e8d-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="35e8d-108">Кроме того, если служба Bing используется в качестве поисковой системы, упреждающее средство проверки подлинности повышает производительность адресной строки и помогает создавать результаты поиска, сопоставленные потребностям вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="35e8d-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="35e8d-109">**Windows Hello Кредуи для проверки подлинности NTLM**</span><span class="sxs-lookup"><span data-stu-id="35e8d-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="35e8d-110">Если единый вход (SSO) недоступен, если веб-сайт пытается войти в систему с помощью механизма NTLM или согласования, эта функция позволит пользователю предоставлять учетные данные ОС на веб-сайте и выполнять проверку подлинности с помощью пользовательского интерфейса Windows Hello cred.</span><span class="sxs-lookup"><span data-stu-id="35e8d-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="35e8d-111">Этот процесс входа будет отображаться только в Windows 10 и только для тех пользователей, которые не получают единый вход во время проверки подлинности NTLM или согласования.</span><span class="sxs-lookup"><span data-stu-id="35e8d-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="35e8d-112">**Использование сохраненных паролей для автоматического входа**</span><span class="sxs-lookup"><span data-stu-id="35e8d-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="35e8d-113">Пользователи, которые сохраняют пароли в Microsoft EDGE, могут включить автоматический вход на веб-сайты, где у них есть сохраненные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="35e8d-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="35e8d-114">Пользователи могут включать и отключать эту функцию в edge://settings/passwords, а также настраивать ее в политиках [диспетчера паролей](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="35e8d-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
