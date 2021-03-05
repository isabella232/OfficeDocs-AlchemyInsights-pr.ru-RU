---
title: Синхронизация пароля
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449143"
---
# <a name="password-synchronization"></a>Синхронизация пароля

**Синхронизация с hash password не работает вообще**

Некоторые распространенные проблемы, с которыми сталкиваются клиенты, когда синхронизация с hash password не работает:

- Учетной записи Active Directory, используемой Azure AD Connect для связи  с локальной  службой Active Directory, не предоставляется изменение каталога репликации, а каталог репликации изменяет все разрешения, необходимые для синхронизации паролей. Это необходимо исправить, выдав эти разрешения учетной записи Active Directory.
- Синхронизация хаширования паролей отключена после того, как  администратор изменил метод user Sign-In с синхронизации паролей на другой вариант, например Federation **с AD FS** в мастере Подключения Azure AD Connect. Это можно исправить, повторно включив функцию синхронизации с **hash** паролей в мастере Подключения Azure AD.
- Проблема подключения с локальной службой Active Directory. Например, некоторые контроллеры домена недоступны Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) или необходимые порты заблокированы брандмауэром. Это необходимо исправить, обеспечив правильное подключение между сервером Azure AD Connect и локальной службой Active Directory.
- Сервер Azure AD Connect в настоящее время находится в режиме постановки, из-за чего серверу не удастся получить хэши паролей. Чтобы устранить проблему, следуйте шагам, описанным в разделе Синхронизация паролей с синхронизацией [Azure AD Connect. Пароли](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)не синхронизируются.

**Синхронизация с hash password не работает для некоторых пользователей**

1. Если вы заметили, что hash паролей не  синхронизируется для пользователя, используйте задачу устранения неполадок в Azure AD Connect для расследования и устранения проблемы. Выполните следующие задачи:

    а) [Выполнить задачу устранения неполадок в мастере](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    б) [Используйте командалет устранения неполадок, чтобы исследовать проблему синхронизации хаши пароля для определенного использования](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Локальное устройство Active Directory User включено для пользователя, который должен изменить пароль **при следующем параметре logon.** Когда этот параметр включен, пользователю назначен временный пароль и ему будет предложено изменить пароль на следующем логотипе. Azure AD Connect не синхронизирует временные пароли с Azure AD.

Чтобы устранить вышеуказанную проблему, выполните любой из следующих задач:

- Попросите пользователя войти в локальное приложение (например, Windows Desktop) и изменить пароль. Новый пароль будет синхронизирован с Azure AD.
- У администратора обновить пароль пользователя без включения параметра **Пользователь** должен изменить пароль на следующем логотипе, и поделиться новым паролем с пользователем.

3. Локально объект Active Directory User  неправильно настроен для синхронизации объектов или синхронизации паролей. Чтобы устранить эту проблему, выполните действия, описанные в синхронизации с помощью синхронизации паролей [с помощью синхронизации Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







