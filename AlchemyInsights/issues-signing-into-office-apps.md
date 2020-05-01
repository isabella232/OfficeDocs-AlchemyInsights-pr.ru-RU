---
title: Проблемы с входом в приложения Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938320"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Исправление приложений Office "доверенный платформенный модуль вашего компьютера не работает должным образом" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Очистите учетные данные Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br/>
    **Примечание:** Пути реестра для Office 2016 изменились на 16,0. (Пример: \Software\Microsoft\Office\16.0\Common\Identity\)
- Попытайтесь выполнить [процесс восстановления пользователей](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , чтобы исправить ошибки ДОВЕРЕНного платформенного модуля.
- Задайте Енаблеадал = 0, выполнив следующие действия:  
    1. Щелкните правой кнопкой мыши Windows Пуск, выберите команду **выполнить**, введите **regedit**и нажмите кнопку **ОК**.
    2. Выберите **Да** , чтобы разрешить редактору реестра вносить изменения на устройстве.
    3. В редакторе реестра добавьте значение DWORD **енаблеадал** с параметром **0** в раздел HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).