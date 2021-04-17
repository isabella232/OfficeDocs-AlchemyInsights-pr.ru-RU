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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826284"
---
# <a name="teams-client-crashing"></a>Сбой клиента Teams?

Если ваш клиент Teams дает сбой, попробуйте следующее:

- Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.

- убедитесь в доступности всех [URL-адресов Microsoft 365 и диапазонов адресов](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Войдите в систему с учетной записью администратора клиента и проверьте [панель мониторинга работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев и снижения качества обслуживания.

- Удалите и повторно установите приложение Teams (ссылка)
    - Перейдите в папку %appdata%\Microsoft\teams\ на вашем компьютере и удалите все файлы в этой папке.
    - [Скачайте и установите приложение Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) и, если это возможно, установите Teams от имени администратора (щелкните правой кнопкой мыши установщик Teams и выберите пункт «Запуск от имени администратора»).

Если в работе клиента Teams по-прежнему возникают сбои, сможете ли вы воспроизвести проблему? Если да:

1. Запишите действия, используя средство записи действий.
    - Закройте все ненужные приложения и приложения, работающие с конфиденциальной информацией.
    - Запустите средство записи действий и воспроизведите проблему, выполнив вход в затронутую учетную запись пользователя.
    - [Соберите журналы команд, которые фиксируют записанные шаги воспроизведения](https://docs.microsoft.com/microsoftteams/log-files). **Примечание**: Убедитесь в том, что вы записали адрес для входа в систему затронутых пользователей.
    - Соберите сведения о дампе и/или сведения о контейнере ошибки (Windows). Запустите Windows PowerShell на компьютере, на котором происходит сбой, и выполните следующие команды:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Вложите файл в ваше обращение в службу поддержки.
