---
title: Сбой клиента Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268785"
---
# <a name="teams-client-crashing"></a>Сбой клиента Teams?

Если ваш клиент Teams дает сбой, попробуйте следующее:

- Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.

- убедитесь в доступности всех [URL-адресов Microsoft 365 и диапазонов адресов](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Войдите в систему с учетной записью администратора клиента и проверьте [панель мониторинга работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев и снижения качества обслуживания.

 - В качестве последнего шага вы можете попытаться очистить кеш клиента вашего Teams:

    1.  Полностью выйдите из настольного клиента Microsoft Teams. Можно щелкнуть правой кнопкой мыши **Teams** в области значков и выбрать команду **закрыть**или запустить диспетчер задач и выполнить полное завершение процесса.

    2.  Перейдите в проводник и введите %appdata%\Microsoft\teams.

    3.  Попав в каталог, вы увидите несколько следующих папок:

         - Из **кеша приложений** перейдите в кеш и удалите все файлы в расположении  %appdata%\Microsoft\teams\application cache\cache.

        - Из **Blob_storage** удалите все файлы: %appdata%\Microsoft\teams\blob_storage.

        - Из **кэша** удалите все файлы: %appdata%\Microsoft\teams\Cache.

        - Из **баз данных** удалите все файлы: %appdata%\Microsoft\teams\databases.

        - Из **GPUCache** удалите все файлы: %appdata%\Microsoft\teams\GPUcache.

        - Изнутри **IndexedDB** удалите файл .db: %appdata%\Microsoft\teams\IndexedDB.

        - Из **локального хранилища** удалите все файлы:%appdata%\Microsoft\teams\Local Storage.

        - Наконец, из **tmp** удалите любой файл:%appdata%\Microsoft\teams\tmp.

    4. Перезапустите клиент Teams.

Если в работе клиента Teams по-прежнему возникают сбои, сможете ли вы воспроизвести проблему? Если да: 

1. Запишите действия, используя средство записи действий.
    - Закройте все ненужные приложения и приложения, работающие с конфиденциальной информацией.
    - Запустите средство записи действий и воспроизведите проблему, выполнив вход в затронутую учетную запись пользователя.
    
2. Вложите файл в ваше обращение в службу поддержки.
