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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972837"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Устранение неполадок, основанных на паролях, проблемы с бесшовным одним входом (SSO)

Чтобы узнать основы SSO на основе [паролей,](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)см. в Azure Active Directory.

**Настройка SSO на основе пароля**

1. [Настройка единого](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) входного знака на основе пароля . В этой статье подробно об этом параметре SSO на основе пароля. Если приложение, которое вы добавляете, требует настраиваемой конфигурации и вам необходимо использовать SSO на основе паролей, то эта статья для вас.
2. [Настройка единого знака](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) на основе паролей для приложений на основе предварительной записи — Прокси-сервер приложения поддерживает несколько режимов входов. Вход на основе пароля предназначен для приложений, которые используют сочетание имени пользователя и пароля для проверки подлинности. При настройке входной записи на основе пароля для приложения пользователям необходимо один раз войти в локальное приложение. После этого Azure Active Directory сохраняет сведения о входе и автоматически предоставляет ее приложению при удаленном доступе пользователей.
    - Вы уже должны были опубликовать и протестировать приложение с помощью прокси-сервера приложения. Если нет, выполните действия в приложениях Публикации с помощью прокси-сервера [приложения Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) а затем продолжите конфигурацию SSO на основе паролей для приложений на основе предварительной записи.

Чтобы устранить проблемы, основанные на паролях, см. в документе Устранение неполадок с одним входом на основе пароля [в Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
