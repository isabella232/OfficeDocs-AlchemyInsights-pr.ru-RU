---
title: Dynamics 365 — неправильная отображение панели мониторинга в едином интерфейсе Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711288"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="96782-102">Неправильное отображение панели мониторинга в едином интерфейсе Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="96782-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="96782-103">Существует несколько причин, по которым может отображаться другая панель мониторинга, отличная от ожидаемой.</span><span class="sxs-lookup"><span data-stu-id="96782-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="96782-104">Пользователь задает панель мониторинга пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="96782-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="96782-105">Как правило, вы можете определить пользовательскую панель мониторинга по умолчанию, **если она не** отображается на панели команд панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="96782-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="96782-106">Панель мониторинга пользователя по умолчанию будет переопределять все остальные панели мониторинга по умолчанию, даже если панель мониторинга пользователя по умолчанию отсутствует в текущем приложении.</span><span class="sxs-lookup"><span data-stu-id="96782-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="96782-107">Используйте приведенное ниже временное решение, чтобы удалить панель мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="96782-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="96782-108">Создайте новую персональную панель мониторинга.</span><span class="sxs-lookup"><span data-stu-id="96782-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="96782-109">Назначение новой панели мониторинга для пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="96782-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="96782-110">Удаление панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="96782-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="96782-111">Панель мониторинга задается на Sitemap</span><span class="sxs-lookup"><span data-stu-id="96782-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="96782-112">Возможно, вы установили панель мониторинга по умолчанию для Организации, выбрав Панель мониторинга и выбрав пункт "по умолчанию" в разделе "Настройка системы".</span><span class="sxs-lookup"><span data-stu-id="96782-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="96782-113">Но панель мониторинга, определенная в конструкторе карт сайтов, будет иметь приоритет над этой панелью мониторинга, если пользователь имеет к ней доступ.</span><span class="sxs-lookup"><span data-stu-id="96782-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="96782-114">Чтобы пользователи видели панель мониторинга, настроенную в качестве организации по умолчанию, можно выполнить одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="96782-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="96782-115">Настройка панели мониторинга в Sitemap</span><span class="sxs-lookup"><span data-stu-id="96782-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="96782-116">Отмена доступа к панели мониторинга, определенной для этих пользователей</span><span class="sxs-lookup"><span data-stu-id="96782-116">Remove access to the sitemap defined dashboard for those users</span></span>
