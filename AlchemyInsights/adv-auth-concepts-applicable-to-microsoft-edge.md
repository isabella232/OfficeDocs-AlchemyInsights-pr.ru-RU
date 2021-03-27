---
title: Расширенные концепции проверки подлинности, применимые к Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398598"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="4c9ab-102">Расширенные концепции проверки подлинности, применимые к Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4c9ab-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="4c9ab-103">Далее ниже следующую концепцию проверки подлинности, применимую к Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="4c9ab-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="4c9ab-104">**Активная проверка подлинности**</span><span class="sxs-lookup"><span data-stu-id="4c9ab-104">**Proactive Authentication**</span></span>

<span data-ttu-id="4c9ab-105">Когда вы включаете политику [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge будет пытаться упреждающие проверки подлинности пользователей с помощью служб Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="4c9ab-106">Через регулярные промежутки времени он будет использовать онлайн-службу для проверки обновленного манифеста, содержающего конфигурацию, управляющую активной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="4c9ab-107">Преимущества. Активная проверка подлинности позволяет проверить подлинность для ключевых служб, таких как страница Office New Tab.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="4c9ab-108">Кроме того, если Bing используется в качестве поисковой системы, активная проверка подлинности повышает производительность панели адресов и помогает создавать результаты поиска, персонализированные для потребностей вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="4c9ab-109">**Windows Hello CredUI для проверки подлинности NTLM**</span><span class="sxs-lookup"><span data-stu-id="4c9ab-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="4c9ab-110">Если один вход (SSO) не доступен, когда веб-сайт пытается подписаться на пользователя с помощью механизма NTLM или Negotiate, эта функция позволит пользователю делиться учетными данными ОС с веб-сайтом и удовлетворять проблему проверки подлинности с помощью пользовательского интерфейса Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="4c9ab-111">Этот поток входов будет отображаться только в Windows 10 и только для пользователей, которые не получают SSO во время NTLM или проблемы Negotiate.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="4c9ab-112">**Использование сохраненных паролей для автоматического включаемой записи**</span><span class="sxs-lookup"><span data-stu-id="4c9ab-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="4c9ab-113">Пользователи, которые сохраняют пароли в Microsoft Edge, могут включить автоматическую запись на веб-сайты, на которых сохранены учетные данные.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="4c9ab-114">Пользователи могут включить или отключить эту функцию в edge://settings/passwords и настроить ее в политиках [диспетчера](https://go.microsoft.com/fwlink/?linkid=2134622) паролей.</span><span class="sxs-lookup"><span data-stu-id="4c9ab-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
