---
title: Синхронизация паролей с устранением неполадок
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105771"
---
# <a name="troubleshoot-password-synchronization"></a>Синхронизация паролей с устранением неполадок

Чтобы устранить проблемы синхронизации паролей, начните с этой задачи Подключение AAD, чтобы определить, почему пароли не синхронизируются. Для начала перейдите к [управлению прямой синхронизацией](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Откройте новый сеанс Windows PowerShell на сервере Azure AD Подключение и выберите параметр **Run as Administrator.**

2. Запуск Set-ExecutionPolicy удаленной или Set-ExecutionPolicy неограниченной.

3. Запустите мастер Azure AD Подключение.

4. Перейдите на страницу Дополнительные задачи > **устранение**  >  **неполадок Далее**.

5. Выберите **Запуск,** чтобы открыть меню устранения неполадок PowerShell.

6. Выберите **синхронизацию паролей устранения неполадок.**

    Обычно проблема в том, что пароль не синхронизируется для определенной учетной записи пользователя.

    **Примечания** Синхронизация паролей не удается, если последняя успешная синхронизация паролей была некоторое время назад.

Дополнительные справки по устранению неполадок синхронизации паролей см. в справке Синхронизация хаши пароля с помощью синхронизации паролей [Azure AD Подключение.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)