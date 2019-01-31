---
title: Устранение неполадок с регистрация Android устройств в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655896"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="4eaba-102">Устранение неполадок с регистрация Android устройств в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4eaba-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="4eaba-103">Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему сейчас.</span><span class="sxs-lookup"><span data-stu-id="4eaba-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="4eaba-104">Некоторые распространенные проблемы и инструкции по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="4eaba-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="4eaba-p101">**Устройство не зашифрованы ошибка в портал компания:** Новая версия Android, начиная с v7.0, особенно требовать секретный код загрузки для убедитесь в том, что полностью шифруются устройства. Типичные решения, чтобы включить ПИН-код запуска или полностью шифрование устройства. Просмотрите [Этот документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="4eaba-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="4eaba-p102">**Устройств не удается проверить с помощью службы Intune или в виде «Неработоспособная» в консоли администрирования Intune:** Некоторые 4.4 Samsung и 5.5 устройств могут не проверять в службу. Существует 3 возможные решения для устранения этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="4eaba-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="4eaba-110">Вручную откройте приложение портала компании Intune автоматически начнет синхронизации устройства.</span><span class="sxs-lookup"><span data-stu-id="4eaba-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="4eaba-111">Обновление устройства Android 6.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="4eaba-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="4eaba-p103">Отключение смарт-диспетчер Samsung от управления портала компании Intune. Просмотрите [Этот документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для получения подробных сведений о эти проблемы и решения.</span><span class="sxs-lookup"><span data-stu-id="4eaba-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="4eaba-p104">**Недопустимый тип лицензии пользователя** или **имя пользователя не распознается ошибки:** пользователь должен быть назначен Intune или Командной лицензии. Просмотрите эти документы назначение лицензии через: центр администрирования Office или Azure портала.</span><span class="sxs-lookup"><span data-stu-id="4eaba-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="4eaba-116">Дополнительные ресурсы, которые помогут устранить проблему:</span><span class="sxs-lookup"><span data-stu-id="4eaba-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4eaba-p105">[Устранение неполадок в портал Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) используйте для диагностики и устранения распространенных ошибок регистрации. Просмотрите [Этот документ](https://docs.microsoft.com/intune/help-desk-operators) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="4eaba-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4eaba-119">Просмотрите [Этот документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) содержит список распространенные ошибки, которые препятствуют регистрации и решения для каждого.</span><span class="sxs-lookup"><span data-stu-id="4eaba-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="4eaba-120">[Узнайте, как зарегистрировать Android устройств в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="4eaba-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

