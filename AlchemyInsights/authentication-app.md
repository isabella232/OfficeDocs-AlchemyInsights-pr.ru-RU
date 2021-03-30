---
title: Приложение проверки подлинности
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403838"
---
# <a name="authentication-app"></a><span data-ttu-id="26cb2-102">Приложение проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="26cb2-102">Authentication app</span></span>

<span data-ttu-id="26cb2-103">Если вы глобальный администратор, вы можете быстро узнать о том, что произошло или диагностировать проблемы, связанные с входом пользователя, с помощью диагностики [входов.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="26cb2-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="26cb2-104">Начните диагностику, нажав кнопку["Запуск](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)диагностики".</span><span class="sxs-lookup"><span data-stu-id="26cb2-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="26cb2-105">Найдите событие для анализа, введите сведения о пользователе, приложении, времени входа, id запроса или корреляции.</span><span class="sxs-lookup"><span data-stu-id="26cb2-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="26cb2-106">Ознакомьтесь с результатами диагностики, отображающими подробные сведения о том, что произошло и какие действия нужно предпринять, чтобы внести изменения.</span><span class="sxs-lookup"><span data-stu-id="26cb2-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="26cb2-107">**Проверьте применимый сценарий:**</span><span class="sxs-lookup"><span data-stu-id="26cb2-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="26cb2-108">Если пользователь не получает push-уведомления в приложении Microsoft Authenticator, убедитесь, что они не показаны под заблокированными пользователями MFA, как описано в Block и [разблокировать пользователей](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="26cb2-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="26cb2-109">Если пользователь не заблокирован для MFA, но не получает push-уведомления, он может открыть приложение Microsoft Authenticator, которое будет тянуть ожидающих запросов на утверждение.</span><span class="sxs-lookup"><span data-stu-id="26cb2-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="26cb2-110">В качестве альтернативного метода регистрации пользователь также может щелкнуть кнопку Войти другим способом и выбрать код проверки из мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="26cb2-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="26cb2-111">Приложение Microsoft Authenticator — единственный доступный метод для многих пользователей.</span><span class="sxs-lookup"><span data-stu-id="26cb2-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="26cb2-112">[Дополнительные новости о по умолчанию безопасности,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [проверка](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) часто задаваемой вопросы и их устранение.</span><span class="sxs-lookup"><span data-stu-id="26cb2-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="26cb2-113">**Рекомендуемые видео**</span><span class="sxs-lookup"><span data-stu-id="26cb2-113">**Recommended Videos**</span></span>

<span data-ttu-id="26cb2-114">[Настройка приложения authenticator на новом телефоне (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="26cb2-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
