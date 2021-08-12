---
title: 646 Настройка AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963656"
---
# <a name="configure-sync-features"></a>Настройка функций синхронизации

Azure AD Подключение включает несколько функций, включенных по умолчанию или которые можно включить позже. Некоторые функции требуют дополнительной конфигурации в определенных средах.

- [Фильтрация](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ограничивает, что объекты синхронизируются с Azure AD. По умолчанию синхронизируются все пользователи, контакты, группы и Windows 10 учетные записи компьютера. Можно включить или исключить объекты, основанные на доменах, OUs или других атрибутах.

- [Синхронизация хаширования паролей](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизируется с хашом пароля из локального Active Directory в Azure AD. Это позволяет использовать управление паролем в одном расположении, но использовать один и тот же пароль как в локальной, так и в облачной среде. Поскольку Active Directory является авторитетным источником, можно использовать собственные политики паролей.

- [Сброс пароля самообслуживающихся (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволяет пользователям сбросить собственные пароли в облаке, применяя при этом политику локального пароля.

- [Списывка](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) устройств позволяет записывать зарегистрированные устройства в Azure AD обратно в локальное Active Directory, чтобы они могли использоваться для условного доступа.

- [Предотвращение случайных удалений](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) включено по умолчанию, чтобы предотвратить слишком много одновременных удалений объектов (более 500 объектов на синхронизацию). Этот параметр можно изменить для удовлетворения потребностей организации.

- [Автоматическое](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) обновление включено по умолчанию для экспресс-установок и помогает обеспечить, чтобы ваша версия Azure AD Подключение всегда была текущей.
