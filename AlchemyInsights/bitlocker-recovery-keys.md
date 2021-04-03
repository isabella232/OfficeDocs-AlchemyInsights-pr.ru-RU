---
title: Ключи восстановления Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505081"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Доступ к клавишам восстановления Bitlocker

При настройке параметров Bitlocker Intune Endpoint Protection Policy можно определить, следует ли хранить сведения о восстановлении Bitlocker в Azure Active Directory.

Если этот параметр настроен, сохраненные данные восстановления должны быть видны администратору Intune в составе данных записи устройства в лезвии Intune Devices двумя способами:

Устройства - устройства Azure AD -> "Device" OR Devices -> Все устройства -> "Device" -> Клавиши восстановления

Кроме того, если имеется административный доступ к самому устройству, ключ восстановления (пароль) можно увидеть, заметив следующую команду из команды с повышенным запросом:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Если устройство было зашифровано до регистрации в Intune, ключ восстановления мог быть связан с "Microsoft Account" (MSA), используемым для входов на устройство во время процесса OOBE. Если это так, доступ и вход с этим MSA должны показывать устройства, для которых  https://onedrive.live.com/recoverykey хранились ключи восстановления.
 
Если устройство было зашифровано в результате конфигурации с помощью групповой политики на основе домена, сведения о восстановлении могут храниться в локальном Active Directory.

Если вы настроили политику защиты конечной точки для хранения ключа восстановления в Azure Active Directory, но ключ для определенного устройства не был загружен, вы можете вызвать отправку, поверив ключ восстановления для этого устройства из консоли MEM. Подробные сведения см. в [материале Rotate BitLocker recovery keys.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

