---
title: 646 как настроить AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499683"
---
# <a name="configure-sync-features"></a>Настройка функции синхронизации.

Подключение Azure AD включает в себя ряд функций, включены по умолчанию, или можно включить более поздней версии. Некоторые функции требуется дополнительная настройка в конкретных средах.
  
- Ограничения для [фильтрации](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) объектов синхронизируются с Azure AD. По умолчанию все пользователи, контакты, группы и Windows 10 компьютера учетные записи синхронизированы. Можно включить или исключить объекты на основе доменов, подразделений или другие атрибуты. 
    
- [Хэш-функции синхронизации паролей](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизирует хэш пароля из локального Active Directory для Azure AD. Это позволяет управление паролями в одном месте, но использовать тот же пароль, как в локальных и облачных средах. Поскольку Active Directory авторитетным источником, можно использовать политик паролей. 
    
- [Самостоятельный сброс пароля (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволяет пользователям сбрасывать собственные пароли в облаке при применении политики паролей для локальной по-прежнему. 
    
- [Обратной записи устройства](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволяет зарегистрированных устройства в Azure AD записи в локальной Active Directory, они могут использоваться для условного доступа. 
    
- [Запретить случайное удаление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) включен по умолчанию для предотвращения удаления слишком большого числа одновременных объектов (более 500 объектов в синхронизации). Можно изменить этот параметр в соответствии с требованиями вашей организации. 
    
- [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) включен по умолчанию для установок express и обеспечивает вашей версии Azure AD подключение всегда является текущим. 
    

