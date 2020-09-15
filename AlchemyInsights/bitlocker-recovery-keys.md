---
title: Ключи восстановления BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685899"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Доступ к ключам восстановления BitLocker

При настройке параметров BitLocker в Intune Endpoint Protection можно определить, следует ли хранить данные восстановления BitLocker в Azure Active Directory.

Если этот параметр настроен, хранимые данные для восстановления должны быть видны администратору Intune в составе данных записи устройства в колонке Intune Devices двумя способами:

Devices — устройства Azure AD — > "устройство" или "устройства" — > все устройства — > "устройство" — ключи восстановления >

Кроме того, если есть административный доступ к самому устройству, можно просмотреть ключ восстановления (пароль), выполнив следующую команду из командной строки с повышенными привилегиями:

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
Если устройство было зашифровано до енролмент в Intune, ключ восстановления мог быть связан с учетной записью Майкрософт (MSA), используемой для входа в устройство во время процесса OOBE. В этом случае при доступе  https://onedrive.live.com/recoverykey и входе в систему с помощью MSA должны отображаться устройства, для которых были сохранены ключи восстановления.
 
Если устройство было зашифровано в результате настройки с помощью групповой политики домена, сведения для восстановления могут храниться в локальной службе Active Directory.
 

