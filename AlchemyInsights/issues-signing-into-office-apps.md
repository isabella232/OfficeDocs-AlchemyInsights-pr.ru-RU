---
title: Проблемы с входом в Microsoft 365 приложения
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986904"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Исправление Microsoft 365 приложения "Модуль доверенных платформ компьютера не функционирует должным образом" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Установка последних обновлений для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [и Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Очистка Office учетных](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) данных с Windows диспетчером учетных данных.<br/>
    **Примечание:** Пути реестра за Office 2016 г. изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Попробуйте [процесс восстановления пользователей,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) чтобы устранить сбои в работе модуля доверенных платформ (TPM).
- Установите EnableADAL = 0 с помощью следующих действий:  
    1. Правой кнопкой мыши нажмите кнопку Windows, выберите **выполнить,** введите **regedit,** а затем выберите **ОК**.
    2. Выберите **Да,** чтобы разрешить редактору реестра вносить изменения в устройство.
    3. В редакторе реестра добавьте значение DWORD **EnableADAL** с параметром **0** в HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Дополнительные сведения см. в документе Проблемы подключения при входе после обновления Office 2016 г. Сборка [16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)на Windows 10 .