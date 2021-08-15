---
title: Устранение неполадок с одним входом для устройств, присоединитых к Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039259"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Устранение неполадок с одним входом для устройств, присоединитых к Azure AD

Если у вас есть локальное окружение Active Directory (AD) и вы хотите присоединиться к компьютерам, присоединимым к домену AD, в Azure AD, вы можете добиться этого путем гибридного пользования Azure AD. [Как: планирование гибридного Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) реализации реализации позволяет выполнить соответствующие действия по внедрению гибридного лазурного AD в вашей среде.

Дополнительные сведения см. в дополнительных сведениях о настройке устройств Azure AD для локального Single-Sign с использованием [Windows Hello для бизнеса.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Основные проблемы маркера обновления (PRT)**

Основной маркер обновления (PRT) — это ключевой артефакт проверки подлинности Azure AD на Windows 10, Windows Server 2016 и более поздних версиях, устройствах iOS и Android. Это веб-маркер JSON (JWT), специально выданный брокерам маркеров первой стороны Майкрософт, чтобы включить единую регистрацию (SSO) в приложениях, используемых на этих устройствах. Сведения о том, как prT выдают, используют и защищают на Windows 10 устройствах, см. в материале [What is a Primary Refresh Token?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: ДА и AzureADPrt: ДА**

В этих полях указывается, успешно ли пользователь прошел проверку подлинности в Azure AD при входе на устройство. Если значения **нет,** это может быть связано с:

- Плохой ключ хранения в TPM, связанный с устройством при регистрации (проверьте KeySignTest при работе с повышенным значением)
- Альтернативный ID входа
- Http Proxy не найден

Для устранения неполадок устройств с помощью команды dsregcmd см. [состояние SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
