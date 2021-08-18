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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088049"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустой экран регистрации в Microsoft 365 приложениях

Чтобы устранить эту проблему, попробуйте следующее:
- Установка последних обновлений для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [и Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Сброс параметров Internet Explorer: Перейдите к средствам Internet  >  **Options**  >  **Advanced**  >  **Reset Internet Explorer Параметры** (обратите внимание, что вы потеряете настраиваемые параметры), а затем попробуйте зарегистрироваться, чтобы Office снова.
- Отключение Application Guard в Защитнике Windows (WDAG) или любого аналогичного брандмауэра или антивирусной программы:
    1. В панели управления перейдите к **программам,** а затем выберите функции **Windows включить или отключить**.
    2. Если Application Guard в Защитнике Windows включена, попробуйте отключить его.<br/>
    **Примечание:** Возможно, потребуется перезапустить компьютер.
- Убедитесь, что подключаемый модуль WAM Microsoft.AAD.BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокируется ни приложением, ни брандмауэром, ни антивирусной программой.
- [Очистка Office учетных](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) данных с Windows диспетчером учетных данных.<br/>
    **Примечание:** Пути реестра за Office 2016 г. изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Дополнительные сведения см. в документе Проблемы подключения при входе после обновления Office 2016 г. Сборка [16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)на Windows 10 .