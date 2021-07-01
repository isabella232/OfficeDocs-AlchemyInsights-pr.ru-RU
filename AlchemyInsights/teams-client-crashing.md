---
title: Сбой клиента Teams?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187734"
---
# <a name="teams-client-crashing"></a>Сбой клиента Teams?

Если ваш клиент Teams дает сбой, попробуйте следующее:

- Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.

- убедитесь в доступности всех [URL-адресов Microsoft 365 и диапазонов адресов](/microsoftteams/connectivity-issues).

- Войдите в систему с учетной записью администратора клиента и проверьте [панель мониторинга работоспособности службы](/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев и снижения качества обслуживания.

- Удалите и повторно установите приложение Teams
    - Перейдите в папку %appdata%\Microsoft\Teams\ на вашем компьютере и удалите все файлы в этой папке.
    - [Скачайте и установите приложение Teams](https://www.microsoft.com/microsoft-teams/download-app) и, если это возможно, установите Teams от имени администратора (щелкните правой кнопкой мыши установщик Teams и выберите пункт **Запуск от имени администратора**).

Если в работе клиента Teams по-прежнему возникают сбои, попробуйте воспроизвести проблему. Если можешь...

1. Запишите действия, используя средство записи действий.
    - Закройте все ненужные приложения и приложения, работающие с конфиденциальной информацией.
    - Запустите средство записи действий и воспроизведите проблему, выполнив вход в затронутую учетную запись пользователя.
    - [Соберите журналы команд, которые фиксируют записанные шаги воспроизведения](/microsoftteams/log-files). **Примечание**: Убедитесь в том, что вы записали адрес для входа в систему затронутых пользователей.
    - Соберите сведения о дампе и/или сведения о контейнере ошибки (Windows). Запустите Windows PowerShell на компьютере, на котором происходит сбой, и выполните следующие команды (нажимая после каждой кнопку ВВОД):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. После того как текстовый файл будет создан и появится на экране, сохраните его и вложите в запрос на обслуживание. 
