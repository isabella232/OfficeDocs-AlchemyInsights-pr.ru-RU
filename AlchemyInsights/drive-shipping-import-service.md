---
title: Доставка дисков в службу импорта Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721724"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Доставка дисков в службу импорта Microsoft 365

Используйте доставку диска, скопировав PST-файлы на жесткий диск, а затем отправив жесткий диск в Microsoft.

Запуск задания:

1. В Центре соответствия требованиям Microsoft 365 в разделе **Управление сведениями** выберите **Импорт**.

1. Выберите **Выбрать тип задания импорта**, а затем нажмите **Далее**.

1. Чтобы увидеть действия для этого варианта импорта, выберите **Доставка жестких дисков по адресу нашего фактического местонахождения**.

Помните:

- Для импорта PST-файлов в почтовые ящики Microsoft 365 необходимо назначить роль экспорта-импорта почтовых ящиков в Exchange Online.
Производительность PTS-файлов размером более 20 ГБ может снизиться.

- Можно использовать только 2,5-дюймовые твердотельные диски (SSD) и 2,5- или 3,5-дюймовые внутренние жесткие диски SATA II/III.
Жесткий диск, содержащий PST-файлы, должен быть зашифрован с помощью BitLocker.

- Стоимость импорта PST-файлов в почтовые ящики Microsoft 365 при отправке жестких дисков в корпорацию Майкрософт составляет 2 доллара США за 1 ГБ данных.

Дополнительные сведения об использовании метода доставки дисков для импорта PST-файлов см. [Использование доставки дисков для импорта PST-файлов вашей организации](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).