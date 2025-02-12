---
title: Параметры запуска в Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909839"
---
# <a name="startup-settings-in-windows-10"></a>Параметры запуска в Windows 10

**Изменение автоматического запуска приложений при запуске**

1. Перейдите [Параметры > приложения > запуска](ms-settings:startupapps?activationSource=GetHelp).

2. Убедитесь, что любое приложение, которое необходимо запустить при запуске, **включено.**

**Добавление приложения для автоматического запуска при запуске**

1. Нажмите кнопку **Пуск** или нажмите кнопку Пуск и найдите приложение, которое необходимо запустить при запуске.

2. Щелкните правой кнопкой мыши приложение, нажмите **кнопку Больше,** а затем нажмите **кнопку Открыть расположение файла**. Это открывает расположение, в котором сохранен ярлык приложения. Если нет возможности для расположения открытого файла, это означает, что приложение не может работать при запуске.

3. С открытым расположением файла нажмите **клавишу Windows + R,** введите оболочку:запуск, а затем нажмите **кнопку ОК**.  Это открывает папку Startup.

4. Скопируйте и вложите ярлык в приложение из расположения файла в папку Startup.

**Расширенные параметры запуска (включая режим Сейф, параметры UEFI и загрузку с другого устройства)**

1. Сохраните работу и закройте все открытые документы, так как эти действия перезапустят компьютер.

2. Перейдите [Параметры > обновления & безопасности > восстановления](ms-settings:recovery?activationSource=GetHelp).

3. В **advanced startup** нажмите **кнопку Перезапустить сейчас**. 

4. После перезапуска компьютера на экран параметра Выберите:

    - Чтобы загрузиться с устройства, например USB-накопителя, нажмите **кнопку Используйте устройство.**

    - Чтобы ввести параметры UEFI (иногда называемую установкой BIOS), нажмите кнопку Устранение неполадок > расширенные параметры > **UEFI Параметры**. 

    - Чтобы ввести режим Сейф или изменить расширенные параметры запуска, нажмите кнопку Устранение неполадок > расширенные параметры > **startup Параметры,** а затем перезапустите .  Возможно, вам будет предложено ввести ключ [восстановления BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) После повторного перезапуска компьютера щелкните параметр запуска, который вы хотите использовать.