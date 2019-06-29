---
title: Устранение неполадок, связанных с регистрацией устройств с Android в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367302"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="eeac7-102">Устранение неполадок, связанных с регистрацией устройств с Android в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="eeac7-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="eeac7-103">Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="eeac7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="eeac7-104">Некоторые распространенные проблемы и способы их устранения.</span><span class="sxs-lookup"><span data-stu-id="eeac7-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="eeac7-105">**Ошибка "устройство не зашифровано" в портале компании:** Более новые версии Android, особенно начиная с версии 7.0, требуют запуска загрузочного кода, чтобы убедиться, что устройство полностью зашифровано.</span><span class="sxs-lookup"><span data-stu-id="eeac7-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="eeac7-106">Общие решения позволяют включить ПИН-код запуска или полностью зашифровать устройство.</span><span class="sxs-lookup"><span data-stu-id="eeac7-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="eeac7-107">Просмотрите [этот документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="eeac7-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="eeac7-108">**Устройства не могут вернуть службу Intune или отобразить как "неработоспособное" в консоли администрирования Intune:** Некоторые устройства Samsung 4,4 и 5,5 могут не вернуть службу.</span><span class="sxs-lookup"><span data-stu-id="eeac7-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="eeac7-109">Существует три возможных решения этой проблемы:</span><span class="sxs-lookup"><span data-stu-id="eeac7-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="eeac7-110">Вручную откройте приложение "Корпоративный портал Intune", которое будет автоматически инициировать синхронизацию устройств.</span><span class="sxs-lookup"><span data-stu-id="eeac7-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="eeac7-111">Обновите устройство до Android 6,0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="eeac7-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="eeac7-112">Отключение интеллектуального менеджера Samsung от управления порталом компании Intune.</span><span class="sxs-lookup"><span data-stu-id="eeac7-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="eeac7-113">Ознакомьтесь с [этим документом](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , чтобы получить дополнительные сведения об этих проблемах и их разрешениях.</span><span class="sxs-lookup"><span data-stu-id="eeac7-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="eeac7-114">**Недопустимый тип лицензии пользователя** , или **имя пользователя не опознано ошибка:** пользователю должна быть назначена лицензия Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="eeac7-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="eeac7-115">Просмотрите эти документы, чтобы назначить лицензию: центр администрирования Office или портал Azure.</span><span class="sxs-lookup"><span data-stu-id="eeac7-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="eeac7-116">Дополнительные материалы по решению возникшей проблемы:</span><span class="sxs-lookup"><span data-stu-id="eeac7-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="eeac7-117">Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации.</span><span class="sxs-lookup"><span data-stu-id="eeac7-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="eeac7-118">Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="eeac7-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="eeac7-119">Просмотрите [этот документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать их.</span><span class="sxs-lookup"><span data-stu-id="eeac7-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="eeac7-120">[Узнайте, как зарегистрировать устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="eeac7-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
