---
title: Проблемы с входом в приложения Microsoft 365
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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579914"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустой экран входа в приложения Microsoft 365

Чтобы устранить эту проблему, попробуйте выполнить следующие действия:
- Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Сброс параметров Internet Explorer: Откройте **меню Сервис**  >  **параметры Internet**  >  **Advanced**  >  **Explorer дополнительно сбросить параметры Internet Explorer** (Обратите внимание, что настраиваемые параметры будут утрачены), а затем попробуйте войти в Office снова.
- Отключите приложение Application Guard в Защитнике Windows (ВДАГ) или аналогичное брандмауэр или антивирусную программу:
    1. В панели управления откройте раздел **программы**, а затем выберите пункт **Включение или отключение компонентов Windows**.
    2. Если включено Application Guard в Защитнике Windows, попробуйте отключить его.<br/>
    **Примечание:** Может потребоваться перезагрузка компьютера.
- Убедитесь, что [подключаемый модуль](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. БРОКЕРПЛУГИН AAD вам не блокируется каким-либо приложением или брандмауэром/антивирусной программой.
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br/>
    **Примечание:** Пути реестра для Office 2016 изменились на 16,0. (Пример: \Software\Microsoft\Office\16.0\Common\Identity\)

Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).