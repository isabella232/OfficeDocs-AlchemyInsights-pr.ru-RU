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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030675"
---
# <a name="teams-client-crashing"></a>Сбой клиента Teams?

Если ваш клиент Teams дает сбой, попробуйте следующее:

- Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.

- Убедитесь, что все [URL-адреса и диапазоны адресов Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступны.

- Войдите в систему под своей учетной записью администратора и проверьте [панель мониторинга работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев или ухудшении качества обслуживания.

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
