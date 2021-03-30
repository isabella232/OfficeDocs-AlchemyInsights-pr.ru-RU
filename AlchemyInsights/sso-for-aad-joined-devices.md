---
title: Single-Sign для устройств Azure Active Directory
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403830"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Единый вход для устройств, присоединив к Azure Active Directory

Если у вас есть локальное окружение Active Directory (AD) и вы хотите присоединиться к компьютерам, присоединимым к домену AD, в Azure AD, вы можете добиться этого путем гибридного пользования Azure AD. [Как: планирование реализации](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) гибридного реализации Azure Active Directory предоставляет вам соответствующие действия по реализации гибридного присоединиться к Azure AD в вашей среде.

[Настройка устройств Azure AD для локального Single-Sign с помощью Windows Hello для бизнеса](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Основные проблемы маркера обновления (PRT)** Основной маркер обновления (PRT) — это ключевой артефакт проверки подлинности Azure AD на устройствах Windows 10, Windows Server 2016 и более поздних версий, iOS и Android. Это веб-маркер JSON (JWT), специально выданный брокерам маркеров первой стороны Майкрософт, чтобы включить единую регистрацию (SSO) в приложениях, используемых на этих устройствах. [В "Что такое основной маркер обновления?",](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)мы предокажим сведения о том, как prT выдают, используют и защищают на устройствах с Windows 10.

**WamDefaultSet: ДА и AzureADPrt: ДА** В этих полях указывается, успешно ли пользователь прошел проверку подлинности в Azure AD при входе на устройство. Если значения **нет,** это может быть связано:

- Плохой ключ хранилища в TPM, связанный с устройством при регистрации (проверьте KeySignTest при работе с повышенным значением).
- Альтернативный ID входа
- Http Proxy не найден

Устройства устранения неполадок с помощью команды dsregcmd - [состояние SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
