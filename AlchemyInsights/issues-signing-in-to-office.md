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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938319"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Пустой экран входа в приложения Office

Чтобы устранить эту проблему, попробуйте выполнить следующие действия:
- Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Сброс параметров Internet Explorer: Откройте **меню Сервис** > **Параметры** > Internet Explorer**Дополнительно** > **сбросить параметры Internet Explorer** (Обратите внимание, что настраиваемые параметры будут утрачены), а затем попробуйте войти в Office снова.
- Отключите приложение Application Guard в Защитнике Windows (ВДАГ) или аналогичное брандмауэр или антивирусную программу:
    1. В панели управления откройте раздел **программы**, а затем выберите пункт **Включение или отключение компонентов Windows**.
    2. Если включено Application Guard в Защитнике Windows, попробуйте отключить его.<br/>
    **Примечание:** Может потребоваться перезагрузка компьютера.
- Убедитесь, что подключаемый модуль Microsoft. AAD. Брокерплугин [AAD вам](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокируется каким-либо приложением или брандмауэром/антивирусной программой.
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br/>
    **Примечание:** Пути реестра для Office 2016 изменились на 16,0. (Пример: \Software\Microsoft\Office\16.0\Common\Identity\)

Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).