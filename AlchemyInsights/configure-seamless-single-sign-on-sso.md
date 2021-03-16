---
title: Настройка бесшовного единого входного знака (SSO)
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/15/2021
ms.locfileid: "50819569"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Настройка бесшовного единого входного знака (SSO)

**Настройка приложений**

1. Необходимо получить значения от поставщика приложений. Вы можете вручную вводить значения или загружать файл метаданных для извлечения значения полей.
2. Многие приложения уже предварительно настроены для работы с Azure AD. Эти приложения перечислены в галерее приложений, которые можно просмотреть при добавлении приложения в клиента Azure AD. Серия [quickstart](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) проходит через процесс.
3. Чтобы создать приложение, не в галерее, можно нажать **кнопку +Создать** собственное приложение и дать имя приложению.
    - По умолчанию он будет выбирать **интеграцию** любых других приложений, которые не находятся в галерее, что является правильным вариантом для приложений, не в галерее.
    - Как только вы нажмете **Создать** после ввода имени приложения, оно создаст новое не-галерное корпоративное приложение.
    - Затем вы можете  перейти к  единому входу в соответствии с управлением этим приложением, и вы сможете увидеть различные методы для его реализации в вашей среде.

**Настройка бесшовных SSO для конкретного приложения**

Для приложений в галерее вы найдете подробные пошаговую инструкцию. Чтобы получить доступ к шагам, вы можете просмотреть список всех учебников по конфигурации приложений в учебниках по конфигурации [приложений SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Настройка SSO на основе SAML**

1. Quickstart. Настройка единого входного приложения на основе [SAML (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)для приложения в клиенте Azure Active Directory (Azure AD).
2. Дополнительные информацию о параметре samL для одного входного знака см. в документе [Understand SamL-based single sign-on.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Чтобы узнать о запросах и ответах на проверку подлинности SAML 2.0, поддерживаемых Azure Active Directory (Azure AD) для единого Sign-On (SSO), см. в протоколе Единой Sign-On [SAML.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Подробнее о создании и настройке единого входного знака на основе SAML (SSO) для приложения в Azure Active Directory (Azure AD) с помощью API Microsoft Graph см. в приложении [Configure SAML-based single sign-on для](https://docs.microsoft.com/graph/application-saml-sso-configure-api)приложения с помощью API Microsoft Graph .
5. Подробнее о том, как Azure AD использует протокол SAML, см. в видеоролике Как платформа удостоверений [Майкрософт использует протокол SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Настройка маркеров и утверждений**

1. [Настройка утверждений, выдаемых в маркере SAML для корпоративных приложений.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Чтобы узнать, как настроить утверждения с помощью PowerShell, см. в обзоре [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Чтобы узнать, как настроить необязательные утверждения, см. в приложении [How to: Provide optional claims to your app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Сведения об использовании атрибутов расширения схемы каталогов для отправки пользовательских данных приложениям в утверждениях маркеров см. в приложении [Using directory schema extension attributes in claims.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Чтобы узнать, как настроить сроки служб маркеров, см. в обзоре [Configurable token lifetimes in the Microsoft identity platform (preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. Настройка политик жизни маркеров [(предварительный просмотр)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - В этой статье мы пройдите по общему сценарию политики, который поможет вам ввести новые правила для срока службы маркера. В этом примере вы узнаете, как создать политику, которая требует от пользователей более частой проверки подлинности в вашем веб-приложении.

**Устранение неполадок конфигурации SSO**

- Часто задающие вопросы о бесшовном едином Sign-On Azure [Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)(Бесшовный SSO), см. в этой рубре.
- Сведения о распространенных проблемах, связанных с бесшовным единым Sign-On Azure Active Directory (Azure AD), см. в документе Устранение неполадок Azure Active Directory Seamless [Single Sign-On.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
