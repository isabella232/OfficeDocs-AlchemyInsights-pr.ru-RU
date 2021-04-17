---
title: Как включить бесшовный SSO
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825744"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="ad1e1-102">Как включить бесшовный SSO</span><span class="sxs-lookup"><span data-stu-id="ad1e1-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="ad1e1-103">Включить бесшовную SSO через [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="ad1e1-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="ad1e1-104">Если вы делаете новую установку Azure AD Connect, выберите [настраиваемый путь установки.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="ad1e1-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="ad1e1-105">На странице **Вход пользователя** выберите параметр **Включить** один вход.</span><span class="sxs-lookup"><span data-stu-id="ad1e1-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="ad1e1-106">Чтобы убедиться, что вы правильно включили бесшовную SSO:</span><span class="sxs-lookup"><span data-stu-id="ad1e1-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="ad1e1-107">Во входе в административный центр [Azure Active Directory](https://aad.portal.azure.com) в качестве глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="ad1e1-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="ad1e1-108">Выберите **Azure Active Directory** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="ad1e1-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="ad1e1-109">Убедитесь, что бесшовная одноавтная входная возможность **включена.**</span><span class="sxs-lookup"><span data-stu-id="ad1e1-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="ad1e1-110">Дополнительные дополнительные информации см. в [документе Azure Active Directory Seamless Single Sign-On: Quick start.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="ad1e1-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  