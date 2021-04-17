---
title: Проблемы с входом в приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833017"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Исправление приложения Microsoft 365 "Модуль доверенных платформ компьютера не функционирует должным образом" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Установка последних обновлений [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.<br/>
    **Примечание:** Пути реестра Office 2016 изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Попробуйте [процесс восстановления пользователей,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) чтобы устранить сбои в работе модуля доверенных платформ (TPM).
- Установите EnableADAL = 0 с помощью следующих действий:  
    1. Щелкните правой кнопкой Запуска Windows, выберите **выполнить,** введите **regedit,** а затем выберите **ОК.**
    2. Выберите **Да,** чтобы разрешить редактору реестра вносить изменения в устройство.
    3. В редакторе реестра добавьте значение DWORD **EnableADAL** с параметром **0** в HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Дополнительные сведения см. в документе Проблемы подключения при входе после обновления [office 2016 сборки 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).