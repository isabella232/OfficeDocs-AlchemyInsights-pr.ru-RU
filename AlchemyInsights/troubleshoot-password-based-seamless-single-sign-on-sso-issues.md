---
title: Устранение неполадок, основанных на паролях, проблемы с бесшовным одним входом (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709503"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="e75a3-102">Устранение неполадок, основанных на паролях, проблемы с бесшовным одним входом (SSO)</span><span class="sxs-lookup"><span data-stu-id="e75a3-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="e75a3-103">Чтобы узнать основы SSO на основе паролей, см. в рублях Проверка подлинности на основе паролей [в Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="e75a3-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="e75a3-104">**Настройка SSO на основе пароля**</span><span class="sxs-lookup"><span data-stu-id="e75a3-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="e75a3-105">[Настройка единого](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) входного знака на основе пароля . В этой статье подробно об этом параметре SSO на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="e75a3-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="e75a3-106">Если приложение, которое вы добавляете, требует настраиваемой конфигурации и вам необходимо использовать SSO на основе паролей, то эта статья для вас.</span><span class="sxs-lookup"><span data-stu-id="e75a3-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="e75a3-107">[Настройка единого знака](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) на основе паролей для приложений на основе предварительной записи — Прокси-сервер приложения поддерживает несколько режимов входов.</span><span class="sxs-lookup"><span data-stu-id="e75a3-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="e75a3-108">Вход на основе пароля предназначен для приложений, которые используют сочетание имени пользователя и пароля для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e75a3-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="e75a3-109">При настройке входной записи на основе пароля для приложения пользователям необходимо один раз войти в локальное приложение.</span><span class="sxs-lookup"><span data-stu-id="e75a3-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="e75a3-110">После этого Azure Active Directory хранит сведения о входе и автоматически предоставляет ее приложению при удаленном доступе пользователей.</span><span class="sxs-lookup"><span data-stu-id="e75a3-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="e75a3-111">Вы уже должны были опубликовать и протестировать приложение с помощью прокси-сервера приложения.</span><span class="sxs-lookup"><span data-stu-id="e75a3-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="e75a3-112">Если нет, выполните действия в приложениях Публикации с помощью прокси-сервера [приложения Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) а затем продолжите конфигурацию SSO на основе паролей для приложений на основе предварительной записи.</span><span class="sxs-lookup"><span data-stu-id="e75a3-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="e75a3-113">Чтобы устранить проблемы, основанные на паролях, см. в документе Устранение неполадок с одним входом на основе пароля [в Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="e75a3-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
