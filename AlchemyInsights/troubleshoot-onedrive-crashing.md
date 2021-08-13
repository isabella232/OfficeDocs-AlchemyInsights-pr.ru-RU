---
title: 'Устранение неполадок с OneDrive: аварийное завершение работы'
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
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921020"
---
# <a name="troubleshoot-onedrive-crashes"></a>Устранение неполадок с OneDrive: аварийное завершение работы

Если OneDrive несколько раз аварийно завершает работу, сделайте следующее для устранения неполадок:

**Проверьте, что разделы реестра не заданы:**

1. Откройте редактор реестра и перейдите в раздел HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Если параметр DisableFileSyncNGSC присутствует и его значение "1", откройте раздел и измените значение на "0".
3. Запуск OneDrive вручную через меню "Пуск" ![Нажмите клавишу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), введите "OneDrive" в поле поиска, а затем выберите классическое приложение OneDrive.

**Сброс OneDrive:**

Примечания.

- Сброс OneDrive отключает все существующие подключения синхронизации (включая личный OneDrive, если была выполнена настройка).
- Сброс OneDrive на компьютере не приведет к потере файлов и данных.

**Чтобы сбросить OneDrive:**

1. Откройте диалоговое окно "Выполнить", нажав клавиши Windows+R.
2. Введите команду %localappdata%\Microsoft\OneDrive\onedrive.exe /reset и нажмите кнопку ОК. Ненадолго может появиться командное окно.
3. Запуск OneDrive вручную через меню "Пуск" ![Нажмите клавишу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), введите "OneDrive" в поле поиска, а затем выберите классическое приложение OneDrive.

Примечания.

- Если вы выбрали вариант синхронизации только некоторых папок перед сбросом, вам потребуется выполнить эти действия еще раз после завершения синхронизации. Дополнительные сведения см. в статье  [Выбор папок OneDrive для синхронизации с компьютером](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .
- Вам потребуется проделать эти шаги для личного OneDrive и OneDrive для бизнеса.