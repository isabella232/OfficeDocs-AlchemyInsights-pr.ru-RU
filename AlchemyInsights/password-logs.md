---
title: Журналы паролей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523092"
---
# <a name="password-logs"></a><span data-ttu-id="30ae7-102">Журналы паролей</span><span class="sxs-lookup"><span data-stu-id="30ae7-102">Password logs</span></span>

<span data-ttu-id="30ae7-103">**У меня возникли проблемы с доступом к журналам аудита сброса пароля**</span><span class="sxs-lookup"><span data-stu-id="30ae7-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="30ae7-104">Чтобы устранить проблемы с доступом к журналам аудита сброса пароля, выполните следующее действие:</span><span class="sxs-lookup"><span data-stu-id="30ae7-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="30ae7-105">Убедитесь, что у вас есть права на просмотр журналов аудита.</span><span class="sxs-lookup"><span data-stu-id="30ae7-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="30ae7-106">Такие права имеют только следующие роли:</span><span class="sxs-lookup"><span data-stu-id="30ae7-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="30ae7-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="30ae7-107">Global administrator</span></span>
 - <span data-ttu-id="30ae7-108">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="30ae7-108">Security administrator</span></span>
 - <span data-ttu-id="30ae7-109">Читатель безопасности</span><span class="sxs-lookup"><span data-stu-id="30ae7-109">Security reader</span></span>

<span data-ttu-id="30ae7-110">**Мне нужно просмотреть все события аудита сброса пароля с момента начального развертывания**</span><span class="sxs-lookup"><span data-stu-id="30ae7-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="30ae7-111">В отчетах за последние 30 дней хранится до 120 000 событий регистрации или сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="30ae7-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="30ae7-112">Это максимально допустимое число для пользовательского интерфейса при загрузке CSV-файла.</span><span class="sxs-lookup"><span data-stu-id="30ae7-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="30ae7-113">1 млн событий доступен через PowerShell.</span><span class="sxs-lookup"><span data-stu-id="30ae7-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="30ae7-114">Дополнительные сведения см. по указанным ниже ссылкам.</span><span class="sxs-lookup"><span data-stu-id="30ae7-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="30ae7-115">События самостоятельного сброса пароля из API отчетов и событий Azure AD</span><span class="sxs-lookup"><span data-stu-id="30ae7-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="30ae7-116">Быстрое скачивание событий регистрации для сброса пароля с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="30ae7-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="30ae7-117">**Мне нужны дополнительные сведения о возможностях создания отчетов о сбросе пароля**</span><span class="sxs-lookup"><span data-stu-id="30ae7-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="30ae7-118">Узнайте, кто регистрируется для сброса или сбрасывает пароль, с помощью журналов аудита сброса пароля Azure AD на портале Azure в разделе **Пользователи и группы**.</span><span class="sxs-lookup"><span data-stu-id="30ae7-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="30ae7-119">Дополнительные сведения см. по указанным ниже ссылкам.</span><span class="sxs-lookup"><span data-stu-id="30ae7-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="30ae7-120">Обзор отчетов о сбросе пароля</span><span class="sxs-lookup"><span data-stu-id="30ae7-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="30ae7-121">Как просматривать отчеты о сбросе пароля на портале Azure</span><span class="sxs-lookup"><span data-stu-id="30ae7-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="30ae7-122">События самостоятельного сброса пароля из API отчетов и событий Azure AD</span><span class="sxs-lookup"><span data-stu-id="30ae7-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="30ae7-123">Быстрое скачивание событий регистрации для сброса пароля с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="30ae7-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


