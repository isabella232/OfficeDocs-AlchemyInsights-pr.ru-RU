---
title: Ключи восстановления Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820299"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="b8c99-102">Доступ к клавишам восстановления Bitlocker</span><span class="sxs-lookup"><span data-stu-id="b8c99-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="b8c99-103">При настройке параметров Bitlocker Intune Endpoint Protection Policy можно определить, следует ли хранить сведения о восстановлении Bitlocker в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8c99-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="b8c99-104">Если этот параметр настроен, сохраненные данные восстановления должны быть видны администратору Intune в составе данных записи устройства в лезвии Intune Devices двумя способами:</span><span class="sxs-lookup"><span data-stu-id="b8c99-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="b8c99-105">Устройства - устройства Azure AD -> "Device" OR Devices -> Все устройства -> "Device" -> Клавиши восстановления</span><span class="sxs-lookup"><span data-stu-id="b8c99-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="b8c99-106">Кроме того, если имеется административный доступ к самому устройству, ключ восстановления (пароль) можно увидеть, заметив следующую команду из команды с повышенным запросом:</span><span class="sxs-lookup"><span data-stu-id="b8c99-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="b8c99-107">Если устройство было зашифровано до регистрации в Intune, ключ восстановления мог быть связан с "Microsoft Account" (MSA), используемым для входов на устройство во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="b8c99-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="b8c99-108">Если это так, доступ и вход с этим MSA должны показывать устройства, для которых  https://onedrive.live.com/recoverykey хранились ключи восстановления.</span><span class="sxs-lookup"><span data-stu-id="b8c99-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="b8c99-109">Если устройство было зашифровано в результате конфигурации с помощью групповой политики на основе домена, сведения о восстановлении могут храниться в локальном Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8c99-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="b8c99-110">Если вы настроили политику защиты конечной точки для хранения ключа восстановления в Azure Active Directory, но ключ для определенного устройства не был загружен, вы можете вызвать отправку, поверив ключ восстановления для этого устройства из консоли MEM.</span><span class="sxs-lookup"><span data-stu-id="b8c99-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="b8c99-111">Подробные сведения см. в [материале Rotate BitLocker recovery keys.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="b8c99-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

