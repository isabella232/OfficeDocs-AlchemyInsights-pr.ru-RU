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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833052"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустой экран регистрации в приложениях Microsoft 365

Чтобы устранить эту проблему, попробуйте следующее:
- Установка последних обновлений [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Сброс параметров Internet Explorer: Перейдите к средствам параметров Internet  >    >  **Advanced**  >  **Reset Internet Explorer Settings** (обратите внимание, что вы потеряете настраиваемые параметры), а затем попробуйте снова входить в Office.
- Отключение Защитник Windows безопасности приложений (WDAG) или любого аналогичного брандмауэра или антивирусной программы:
    1. В панели управления перейдите к **программам,** а затем выберите включить или отключить функции **Windows.**
    2. Если Защитник Windows включена охрана приложений, попробуйте отключить ее.<br/>
    **Примечание:** Возможно, потребуется перезапустить компьютер.
- Убедитесь, что подключаемый модуль WAM Microsoft.AAD.BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокируется ни приложением, ни брандмауэром, ни антивирусной программой.
- [Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.<br/>
    **Примечание:** Пути реестра Office 2016 изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Дополнительные сведения см. в документе Проблемы подключения при входе после обновления [office 2016 сборки 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).