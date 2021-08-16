---
title: Проблемы с утверждениями и атрибутами маркеров
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012897"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблемы с утверждениями и атрибутами маркеров

**Обновление, настройка или удаление утверждений маркеров**

1. С помощью Azure Active Directory Azure AD можно [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) настроить тип утверждения для утверждения роли в маркере ответа, который вы получаете после авторизации приложения.
2. Разработчики приложений могут использовать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения они хотят в маркерах, отправленных в их приложение. Дополнительные сведения см. в [приложении Provide optional claims to your app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Настройка групповых утверждений для приложений с помощью Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. При использовании бесшовного единого входного знака в приложении см. в документе настройка утверждений, выдаемых в [маркере SAML для корпоративных приложений.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Сопоставление атрибутов утверждений**

1. Чтобы настроить политику сопоставления утверждений с помощью PowerShell, см. в приложении [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Атрибуты расширения схемы каталогов предоставляют способ хранения дополнительных данных в Azure Active Directory объектах пользователей и других объектах каталога, таких как группы, сведения об клиентах, директорах служб. Только атрибуты расширения на объектах пользователей можно использовать для излучания утверждений в приложениях. [Использование атрибутов](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) расширения схемы каталогов в утверждениях описывает использование атрибутов расширения схемы каталогов для отправки данных пользователей приложениям в утверждениях маркеров.

Дополнительные сведения о утверждениях маркеров см. в:

- [Утверждения в маркерах доступа](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Утверждения в id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Утверждения,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) которые можно ожидать в маркерах ID и маркерах доступа, выданных Azure AD B2C
- [Ссылка на ссылку на утверждения маркера SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
