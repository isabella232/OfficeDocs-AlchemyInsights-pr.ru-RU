---
title: 646 как настроить AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399784"
---
# <a name="configure-sync-features"></a>Настройка функций синхронизации

Azure AD Connect включает несколько функций, которые включены по умолчанию или могут быть включены позже. Для некоторых функций требуется дополнительная настройка в определенных средах.

- Ограничивающие [фильтры](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) объекты синхронизируются с Azure AD. По умолчанию синхронизируются все пользователи, контакты, группы и учетные записи компьютеров с Windows 10. Вы можете включить или исключить объекты, основанные на доменах, подРазделениях и других атрибутах.

- [Хэш пароля синкронизатион](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизирует хэш пароля из локального каталога Active Directory с Azure AD. Это позволяет управлять паролями в одном месте, но использовать один и тот же пароль в локальной и облачной средах как в локальной среде, так и в облачной среде. Так как Active Directory является достоверным источником, вы можете использовать собственные политики паролей.

- [Самостоятельный сброс паролей (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволяет пользователям сбрасывать собственные пароли в облаке, не применяя локальную политику паролей.

- [Обратная запись устройства](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволяет записывать зарегистрированные устройства в Azure AD обратно в локальную службу Active Directory, чтобы их можно было использовать для условного доступа.

- [Защита от случайных удалений](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) включена по умолчанию для предотвращения слишком большого числа одновременных удалений объектов (более 500 объектов в каждой синхронизации). Этот параметр можно изменить в соответствии с потребностями Организации.

- [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) включено по умолчанию для Экспресс-установок и помогает убедиться в том, что ваша версия Azure AD Connect всегда актуальна.
