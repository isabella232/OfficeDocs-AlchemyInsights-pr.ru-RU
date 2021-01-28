---
title: Проблемы с утверждениями и атрибутами маркера
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029990"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблемы с утверждениями и атрибутами маркера

**Обновление, настройка и удаление утверждений маркеров**

1. С помощью Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) можно настроить тип утверждения роли в маркере ответа, который вы получаете после авторизации приложения.
2. Разработчики приложений могут использовать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения они хотят использовать в маркерах, от отправленных приложению. Дополнительные сведения см. в [подзагодии "Предоставление необязательных утверждений для вашего приложения".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Настройка групповых утверждений для приложений с помощью Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. При использовании простого единого вход в приложении см. настройки утверждений, выдаемых в [маркере SAML для корпоративных приложений.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Сопоставление атрибутов утверждений**

1. Чтобы настроить политику сопоставления утверждений с помощью PowerShell, см. "Настройка утверждений, выдаваемых в маркерах для определенного приложения в клиенте [(предварительная версия)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)".
2. Атрибуты расширения схемы каталогов предоставляют способ хранения дополнительных данных в Azure Active Directory для объектов пользователей и других объектов каталогов, таких как группы, сведения о клиенте, основные службы. Только атрибуты расширения в объектах-пользователях можно использовать для выдания утверждений приложениям. [Использование атрибутов](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) расширения схемы каталогов в утверждениях описывает использование атрибутов расширения схемы каталогов для отправки пользовательских данных приложениям в утверждениях маркеров.

Дополнительные сведения об утверждениях маркеров см. в:

- [Утверждения в маркерах доступа](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Утверждения в id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Утверждения,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) которые можно ожидать в маркерах ID и маркерах доступа, выдав azure AD B2C
- [Справочник по утверждениям маркеров SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
