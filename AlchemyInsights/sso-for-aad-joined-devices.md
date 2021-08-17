---
title: Single-Sign для Azure Active Directory присоединились устройства
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050023"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Один вход для Azure Active Directory устройств

Если у вас есть локальное окружение Active Directory (AD) и вы хотите присоединиться к компьютерам, присоединимым к домену AD, в Azure AD, вы можете добиться этого путем гибридного пользования Azure AD. [Как: планирование гибридного Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) реализации реализации позволяет выполнить соответствующие действия по внедрению гибридного лазурного AD в вашей среде.

[Настройка устройств Azure AD для локального Single-Sign При использовании Windows Hello для бизнеса](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Основные проблемы маркера обновления (PRT)** Основной маркер обновления (PRT) — это ключевой артефакт проверки подлинности Azure AD на Windows 10, Windows Server 2016 и более поздних версиях, устройствах iOS и Android. Это веб-маркер JSON (JWT), специально выданный брокерам маркеров первой стороны Майкрософт, чтобы включить единую регистрацию (SSO) в приложениях, используемых на этих устройствах. [В "Что такое основной маркер обновления?",](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)мы предокажим сведения о том, как prT выдан, использован и защищен на Windows 10 устройствах.

**WamDefaultSet: ДА и AzureADPrt: ДА** В этих полях указывается, успешно ли пользователь прошел проверку подлинности в Azure AD при входе на устройство. Если значения **нет,** это может быть связано:

- Плохой ключ хранилища в TPM, связанный с устройством при регистрации (проверьте KeySignTest при работе с повышенным значением).
- Альтернативный ID входа
- Http Proxy не найден

Устройства устранения неполадок с помощью команды dsregcmd - [состояние SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
