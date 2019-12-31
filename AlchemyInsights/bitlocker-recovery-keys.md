---
title: Ключи восстановления BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908827"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="0606d-102">Доступ к ключам восстановления BitLocker</span><span class="sxs-lookup"><span data-stu-id="0606d-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="0606d-103">При настройке параметров BitLocker в Intune Endpoint Protection можно определить, следует ли хранить данные восстановления BitLocker в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0606d-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="0606d-104">Если этот параметр настроен, хранимые данные для восстановления должны быть видны администратору Intune в составе данных записи устройства в колонке Intune Devices двумя способами:</span><span class="sxs-lookup"><span data-stu-id="0606d-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="0606d-105">Devices — устройства Azure AD — > "устройство" или "устройства" — > все устройства — > "устройство" — ключи восстановления ></span><span class="sxs-lookup"><span data-stu-id="0606d-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="0606d-106">Кроме того, если есть административный доступ к самому устройству, можно просмотреть ключ восстановления (пароль), выполнив следующую команду из командной строки с повышенными привилегиями:</span><span class="sxs-lookup"><span data-stu-id="0606d-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="0606d-107">Если устройство было зашифровано до енролмент в Intune, ключ восстановления мог быть связан с учетной записью Майкрософт (MSA), используемой для входа в устройство во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="0606d-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="0606d-108">В этом случае при доступе https://onedrive.live.com/recoverykey и входе в систему с помощью MSA должны отображаться устройства, для которых были сохранены ключи восстановления.</span><span class="sxs-lookup"><span data-stu-id="0606d-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="0606d-109">Если устройство было зашифровано в результате настройки с помощью групповой политики домена, сведения для восстановления могут храниться в локальной службе Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0606d-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

