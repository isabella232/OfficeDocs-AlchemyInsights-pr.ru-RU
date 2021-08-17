---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043219"
---
# <a name="how-to-import-nk2-files"></a>Импорт файлов .nk2 

При первом запуске Microsoft Outlook 2013, Outlook 2016, Outlook 2019 или Outlook для Microsoft 365 года кэш псевдонима (хранится в файле *profilename*.nk2) импортируется в скрытое сообщение в хранилище сообщений по умолчанию.

Чтобы импортировать файлы .nk2 в Outlook 2013, Outlook 2016, Outlook 2019 или Outlook для Microsoft 365, убедитесь, что файл .nk2 находится в следующей папке: %appdata%\Microsoft\Outlook

**Примечание.** Файл .nk2 должен иметь то же имя, что и текущий Outlook 2013 или Outlook 2016 профиль. По умолчанию имя профиля является "Outlook". Чтобы проверить имя профиля, выполните следующие действия: 
1. Нажмите кнопку **Пуск** и выберите **Панель управления**.
2. Дважды нажмите **кнопку Почта**.
3. В диалоговом окне Настройка почты выберите **Показать профили.**
4. Щелкните последовательно **Пуск** > **Выполнить**.
5. В поле **Open** введите *outlook.exe/importnk2,* а затем выберите **ОК.** 

После импорта файла .nk2 содержимое файла сливаются в существующий кэш ником, хранимым в почтовом ящике.

**Примечание.** Файл .nk2 переименован с расширением .old file name при следующем запуске Outlook 2013, Outlook 2016, Outlook 2019 или Outlook для Microsoft 365. Если необходимо повторно импортировать файл .nk2, сначала удалите расширение .old file name.

Дополнительные сведения см. в [примере Import или copy the Auto-Complete List to another computer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)