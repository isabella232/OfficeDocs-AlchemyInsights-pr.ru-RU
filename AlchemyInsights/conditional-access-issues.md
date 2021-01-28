---
title: Проблемы условного доступа
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013978"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="c7fd5-102">Проблемы условного доступа</span><span class="sxs-lookup"><span data-stu-id="c7fd5-102">Conditional access issues</span></span>

<span data-ttu-id="c7fd5-103">**Устранение проблем с диагностикой входа**</span><span class="sxs-lookup"><span data-stu-id="c7fd5-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="c7fd5-104">Вы можете быстро узнать, что произошло или диагностировать проблемы, связанные с входом пользователя, с помощью диагностики [при входе:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="c7fd5-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="c7fd5-105">Запустите Диагностику входа.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="c7fd5-106">Найдите событие для анализа, введите сведения о пользователе, приложении, времени входа, ид запроса или ид корреляции.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="c7fd5-107">Просмотрите результаты диагностики с подробными сведениями о том, что произошло и какие действия можно принять для внесения изменений (если необходимы какие-либо изменения).</span><span class="sxs-lookup"><span data-stu-id="c7fd5-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="c7fd5-108">**Действия по устранению неполадок при входе**</span><span class="sxs-lookup"><span data-stu-id="c7fd5-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="c7fd5-109">Перейдите на страницу входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="c7fd5-110">Фильтрация входов по пользователю, диапазону времени, приложению, статусу, клиентского приложения и так далее.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="c7fd5-111">Выберите событие для регистрации и переберись на вкладку "Условный доступ", чтобы узнать, какие политики были оценены.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="c7fd5-112">Щелкните строку политики, чтобы просмотреть сведения о политике и понять, почему она применяется.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="c7fd5-113">**Средства устранения неполадок политики условного доступа**</span><span class="sxs-lookup"><span data-stu-id="c7fd5-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="c7fd5-114">Режим только для отчетов позволяет оценить политику, не влияя на пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="c7fd5-115">Средство "что-если" позволяет имитировать события входов и видеть, какие политики применяются.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="c7fd5-116">В книге "Анализ и отчеты" отображается влияние каждой политики в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="c7fd5-117">**Базовые политики защиты**</span><span class="sxs-lookup"><span data-stu-id="c7fd5-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="c7fd5-118">Политики базовой защиты были неподготовлены.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="c7fd5-119">Они больше не применяются и скоро будут удалены с портала Azure.</span><span class="sxs-lookup"><span data-stu-id="c7fd5-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="c7fd5-120">Мы рекомендуем включить [значения по умолчанию для системы безопасности.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="c7fd5-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="c7fd5-121">Дополнительные сведения об условном доступе см. в:</span><span class="sxs-lookup"><span data-stu-id="c7fd5-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="c7fd5-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Элементы управления в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Расположения в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="c7fd5-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
