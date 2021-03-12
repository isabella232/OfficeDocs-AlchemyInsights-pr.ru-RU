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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Устранение неполадок, основанных на паролях, проблемы с бесшовным одним входом (SSO)

Чтобы узнать основы SSO на основе паролей, см. в рублях Проверка подлинности на основе паролей [в Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Настройка SSO на основе пароля**

1. [Настройка единого](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) входного знака на основе пароля . В этой статье подробно об этом параметре SSO на основе пароля. Если приложение, которое вы добавляете, требует настраиваемой конфигурации и вам необходимо использовать SSO на основе паролей, то эта статья для вас.
2. [Настройка единого знака](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) на основе паролей для приложений на основе предварительной записи — Прокси-сервер приложения поддерживает несколько режимов входов. Вход на основе пароля предназначен для приложений, которые используют сочетание имени пользователя и пароля для проверки подлинности. При настройке входной записи на основе пароля для приложения пользователям необходимо один раз войти в локальное приложение. После этого Azure Active Directory хранит сведения о входе и автоматически предоставляет ее приложению при удаленном доступе пользователей.
    - Вы уже должны были опубликовать и протестировать приложение с помощью прокси-сервера приложения. Если нет, выполните действия в приложениях Публикации с помощью прокси-сервера [приложения Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) а затем продолжите конфигурацию SSO на основе паролей для приложений на основе предварительной записи.

Чтобы устранить проблемы, основанные на паролях, см. в документе Устранение неполадок с одним входом на основе пароля [в Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
