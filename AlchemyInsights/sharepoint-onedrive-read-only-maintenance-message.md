---
title: Сообщение "только для чтения" для обслуживания при попытке использовать SharePoint или OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840528"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7e284-102">Сообщение "только для чтения" для обслуживания при попытке использовать SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="7e284-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7e284-103">При попытке использовать SharePoint или OneDrive пользователи могут получить сообщение об **обслуживании, доступное только для чтения** .</span><span class="sxs-lookup"><span data-stu-id="7e284-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="7e284-104">Если это так, убедитесь, что в клиенте есть активное обслуживание, перейдя в [Центр сообщений](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="7e284-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="7e284-105">Кроме того, убедитесь, что на панели мониторинга [работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth) есть рекомендации и происшествия, которые могут возникать.</span><span class="sxs-lookup"><span data-stu-id="7e284-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="7e284-106">Если ни центр сообщений, ни панель мониторинга работоспособности службы не отметили ничего о текущем обслуживании клиента, это может быть вызвано ошибкой кэширования браузера.</span><span class="sxs-lookup"><span data-stu-id="7e284-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="7e284-107">Перед переходом на сайт попробуйте очистить кэш браузера.</span><span class="sxs-lookup"><span data-stu-id="7e284-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7e284-108">В браузере Microsoft Edge выберите **Параметры**, а затем выберите **Конфиденциальность и безопасность**.</span><span class="sxs-lookup"><span data-stu-id="7e284-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7e284-109">В разделе **очистить обзор**выберите **команду выбрать, что нужно очистить**.</span><span class="sxs-lookup"><span data-stu-id="7e284-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7e284-110">Выберите **файлы cookie и сохраненные данные веб-сайта**, а затем нажмите кнопку **очистить**.</span><span class="sxs-lookup"><span data-stu-id="7e284-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7e284-111">Эти действия могут отличаться при использовании других браузеров, таких как Mozilla Firefox или Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="7e284-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7e284-112">Кроме того, можно открыть сайт SharePoint или OneDrive в новом окне InPrivate.</span><span class="sxs-lookup"><span data-stu-id="7e284-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>