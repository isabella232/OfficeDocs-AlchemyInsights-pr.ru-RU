---
title: Ошибки конфигурации единого входа
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: 5ab56ec1eda10ea059e600e8933ce85bb143b76e
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886911"
---
# <a name="sso-configuration-issues"></a><span data-ttu-id="c04a3-102">Ошибки конфигурации единого входа</span><span class="sxs-lookup"><span data-stu-id="c04a3-102">SSO configuration issues</span></span>

1. <span data-ttu-id="c04a3-103">Следуйте инструкциям, приведенным в статье [Краткое руководство: Настройка свойств приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure), чтобы настроить приложение.</span><span class="sxs-lookup"><span data-stu-id="c04a3-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="c04a3-104">В зависимости от приложения и выбранного [варианта единого входа](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options), выполните следующие действия: а.</span><span class="sxs-lookup"><span data-stu-id="c04a3-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) that you chose, follow the appropriate guidance below: a.</span></span> <span data-ttu-id="c04a3-105">Чтобы настроить **локальное приложение** для **единого входа на основе SAML**, см. статью [Единый вход SAML для локальных приложений с использованием прокси-сервера приложений](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span><span class="sxs-lookup"><span data-stu-id="c04a3-105">To configure an **on-premises application** for **SAML-based single sign-on (SSO)**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    <span data-ttu-id="c04a3-106">б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-106">b.</span></span> <span data-ttu-id="c04a3-107">Чтобы настроить **облачное приложение** для **единого входа на основе паролей**, см. статью [Настройка единого входа с помощью пароля](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="c04a3-107">To configure a **cloud application** for **password-based SSO**, see [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    <span data-ttu-id="c04a3-108">в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-108">c.</span></span> <span data-ttu-id="c04a3-109">Чтобы настроить **локальное приложение** для **единого входа через прокси-сервер приложения**, см. статью [Настройка хранилища паролей для единого входа с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="c04a3-109">To configure an **on-premises application** for **SSO through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="c04a3-110">**Устранение неполадок, связанных с прокси-сервером приложения**. Рекомендуется начать с изучения процесса устранения неполадок в статье [Отладка проблем с соединителем прокси-сервера ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), чтобы определить, правильно ли настроены соединители прокси-сервера приложения..</span><span class="sxs-lookup"><span data-stu-id="c04a3-110">**Troubleshooting Application Proxy issues**: We recommend that you start with reviewing the troubleshooting flow - [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) - to determine if application proxy connectors are configured correctly.</span></span> <span data-ttu-id="c04a3-111">Если у вас по-прежнему возникают проблемы с подключением к приложению, выполните действия по устранению неполадок в статье [Отладка проблем с прокси приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="c04a3-111">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="c04a3-112">Вы можете [определить ошибки CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues), выполнив следующие действия по отладке браузера:</span><span class="sxs-lookup"><span data-stu-id="c04a3-112">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by performing the following browser debug steps: a.</span></span> <span data-ttu-id="c04a3-113">Запустите браузер и перейдите в веб-приложение.</span><span class="sxs-lookup"><span data-stu-id="c04a3-113">Launch the browser and browse to the web app.</span></span>
    <span data-ttu-id="c04a3-114">б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-114">b.</span></span> <span data-ttu-id="c04a3-115">Нажмите клавишу **F12**, чтобы вывести консоль отладки.</span><span class="sxs-lookup"><span data-stu-id="c04a3-115">Press **F12** to bring up the debug console.</span></span>
    <span data-ttu-id="c04a3-116">в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-116">c.</span></span> <span data-ttu-id="c04a3-117">Попробуйте воспроизвести транзакцию и посмотреть сообщение консоли.</span><span class="sxs-lookup"><span data-stu-id="c04a3-117">Try to reproduce the transaction and review the console message.</span></span> <span data-ttu-id="c04a3-118">Нарушение CORS вызывает консольную ошибку о происхождении.</span><span class="sxs-lookup"><span data-stu-id="c04a3-118">A CORS violation produces a console error about origin.</span></span>
    <span data-ttu-id="c04a3-119">г.</span><span class="sxs-lookup"><span data-stu-id="c04a3-119">d.</span></span> <span data-ttu-id="c04a3-120">Некоторые проблемы CORS невозможно решить, например истечение срока действия маркера доступа, когда приложение перенаправляется на login.microsoftonline.com для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c04a3-120">Some CORS issues can't be resolved, such as expiration of the access token when your app redirects to login.microsoftonline.com for authentication.</span></span> <span data-ttu-id="c04a3-121">В результате истечения срока действия маркера доступа, вызов CORS завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="c04a3-121">As a result of the access token expiration, the CORS call then fails.</span></span> <span data-ttu-id="c04a3-122">Временное решение для этого сценария — продлить жизненный цикл маркера доступа, чтобы предотвратить истечение его срока действия в течении сеанса пользователя.</span><span class="sxs-lookup"><span data-stu-id="c04a3-122">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="c04a3-123">Дополнительные сведения о том, как это сделать, см. в статье [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="c04a3-123">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="c04a3-124">**Устранение неполадок единого входа на основе SAML**. Рекомендуется ознакомиться со статьей [Проблемы со входом в настраиваемые приложения с поддержкой единого входа на основе SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), чтобы найти решения наиболее распространенных проблем.</span><span class="sxs-lookup"><span data-stu-id="c04a3-124">**Troubleshooting SAML-based SSO**: We recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="c04a3-125">**Устранение неполадок единого входа на основе паролей**. Рекомендуется ознакомиться со статьей [Устранение неполадок с единым входом на основе паролей в Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), чтобы найти решения наиболее распространенных проблем.</span><span class="sxs-lookup"><span data-stu-id="c04a3-125">**Troubleshooting password-based SSO**: We recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="c04a3-126">**Произошла ошибка конфигурации**. Чтобы устранить ошибки конфигурации, рекомендуем ознакомиться со статьями ниже.</span><span class="sxs-lookup"><span data-stu-id="c04a3-126">**I received a configuration error**: To troubleshoot configuration errors, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-127">[Проблемы со входом в приложения на основе SAML, настроенные на единый вход.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-127">[Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b.</span></span> <span data-ttu-id="c04a3-128">[Учетные данные заполнены, но расширение не отправляет их](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-128">[Credentials are filled in, but the extension does not submit them](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c.</span></span> <span data-ttu-id="c04a3-129">[Учетные данные заполнены и отправлены, но на странице указано, что учетные данные неверны](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) г.</span><span class="sxs-lookup"><span data-stu-id="c04a3-129">[Credentials are filled in and submitted, but the page indicates the credentials are incorrect](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d.</span></span> [<span data-ttu-id="c04a3-130">На странице приложения выводится сообщение об ошибке после входа пользователя</span><span class="sxs-lookup"><span data-stu-id="c04a3-130">An app page shows an error message after the user signs in</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. <span data-ttu-id="c04a3-131">**Проблемы с интеграцией простого единого входа в локальных приложениях**. Чтобы устранить проблемы, связанные с интеграцией простого единого входа в локальных приложениях, рекомендуем ознакомиться со статьями ниже: а.</span><span class="sxs-lookup"><span data-stu-id="c04a3-131">**I am having issues integrating Seamless SSO with my on-premises apps**: To troubleshoot issues regarding integration of Seamless SSO with on-premises apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-132">[Настройка единого входа в прокси приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-132">[How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b.</span></span> <span data-ttu-id="c04a3-133">[Единый вход SAML для локальных приложений с прокси-сервером](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-133">[SAML single sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c.</span></span> <span data-ttu-id="c04a3-134">[Сведенья об устранении проблем с CORS прокси-сервера приложения Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) г.</span><span class="sxs-lookup"><span data-stu-id="c04a3-134">[Understand and solve Azure Active Directory Application Proxy CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d.</span></span> [<span data-ttu-id="c04a3-135">Устранение неполадок с настойками ограниченного делегирования Kerberos для прокси-сервера приложения</span><span class="sxs-lookup"><span data-stu-id="c04a3-135">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. <span data-ttu-id="c04a3-136">**Мне нужно исправить утверждения или продлить срок действия маркера. Мне нужно изменить продолжительность сеанса**. Для этого рекомендуется ознакомиться со статьями ниже: а.</span><span class="sxs-lookup"><span data-stu-id="c04a3-136">**I need to fix the claims or extend the lifetime of a token. I need to change the length of a session**: To do this, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-137">[Настройка утверждений SAML, отправленных приложению](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-137">[Customize SAML claims sent to an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b.</span></span> <span data-ttu-id="c04a3-138">[Работа с приложениями, поддерживающими утверждения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-138">[Working with claims-aware apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c.</span></span> <span data-ttu-id="c04a3-139">[Настраиваемый жизненный цикл маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) г.</span><span class="sxs-lookup"><span data-stu-id="c04a3-139">[Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d.</span></span> <span data-ttu-id="c04a3-140">[Настройка управления сеансом проверки подлинности с помощью условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) д.</span><span class="sxs-lookup"><span data-stu-id="c04a3-140">[Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e.</span></span> [<span data-ttu-id="c04a3-141">Параметры файлов cookie для доступа к локальным приложениям</span><span class="sxs-lookup"><span data-stu-id="c04a3-141">Cookie settings for accessing on-premises applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. <span data-ttu-id="c04a3-142">**Мне нужна помощь в управлении доступом пользователей и гостей (B2B)**. Подробные сведения об управлении доступом для пользователей и гостей, рекомендуется см. в следующих статьях: а. </span><span class="sxs-lookup"><span data-stu-id="c04a3-142">**I need help managing my user's and guest users' (B2B) access**: For detailed information on managing user's and guest user's access, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-143">[Управление доступом к приложениям](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-143">[Managing access to apps](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b.</span></span> <span data-ttu-id="c04a3-144">[Управление назначением пользователей для приложений в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-144">[Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c.</span></span> <span data-ttu-id="c04a3-145">[Настройка приложений SaaS для совместной работы B2B](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) г.</span><span class="sxs-lookup"><span data-stu-id="c04a3-145">[Configure SaaS apps for B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d.</span></span> <span data-ttu-id="c04a3-146">[Предоставление доступа пользователям B2B в Azure AD к локальным приложениям](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) д.</span><span class="sxs-lookup"><span data-stu-id="c04a3-146">[Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e.</span></span> [<span data-ttu-id="c04a3-147">Предоставление доступа локально управляемым партнерским учетным записям к облачным ресурсам с использованием совместной работы B2B службы Azure AD</span><span class="sxs-lookup"><span data-stu-id="c04a3-147">Grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration</span></span>](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. <span data-ttu-id="c04a3-148">**Я хочу настроить приложения**. Подробные сведения о настройке приложений см. в следующих статьях: а.</span><span class="sxs-lookup"><span data-stu-id="c04a3-148">**I want to customize my apps**: For detailed information on customizing apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-149">[Настройка пользовательских доменов с помощью прокси-сервера приложения Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-149">[Configure custom domains with Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b.</span></span> <span data-ttu-id="c04a3-150">[Установка пользовательской домашней страницы для опубликованных приложений](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) в.</span><span class="sxs-lookup"><span data-stu-id="c04a3-150">[Set a custom home page for published apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c.</span></span> [<span data-ttu-id="c04a3-151">Приложения с подстановочными знаками</span><span class="sxs-lookup"><span data-stu-id="c04a3-151">Wildcard applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. <span data-ttu-id="c04a3-152">**У меня возникают проблемы с переносом приложения из AD FS в Azure**. Чтобы устранить неполадки, возникающие во время миграции приложения из AD FS в Azure, рекомендуется ознакомиться со статьями: а.</span><span class="sxs-lookup"><span data-stu-id="c04a3-152">**I'm having issues migrating my app from AD FS to Azure**: To troubleshoot issues encountered during migration of your app from AD FS to Azure, we recommend checking the following articles: a.</span></span> <span data-ttu-id="c04a3-153">[Перенос проверки подлинности приложения из служб федерации Active Directory в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) б.</span><span class="sxs-lookup"><span data-stu-id="c04a3-153">[Moving application authentication from Active Directory Federation Services to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b.</span></span> [<span data-ttu-id="c04a3-154">Ресурсы для переноса приложений в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c04a3-154">Resources for migrating applications to Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)
