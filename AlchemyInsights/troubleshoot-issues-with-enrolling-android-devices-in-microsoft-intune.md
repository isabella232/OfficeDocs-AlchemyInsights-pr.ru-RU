---
title: Устранение неполадок с регистрацией устройств Android в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709011"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6b2fb-102">Устранение неполадок с регистрацией устройств Android в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6b2fb-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6b2fb-103">Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6b2fb-104">Некоторые распространенные проблемы и действия по разрешению:</span><span class="sxs-lookup"><span data-stu-id="6b2fb-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6b2fb-105">**Ошибка устройства, не зашифрованная на портале компании:** Новые версии Android, особенно начиная с v7.0, требуют запуска пароля, чтобы убедиться, что ваше устройство полностью зашифровано.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="6b2fb-106">Распространенные решения — включить пин-код запуска или полностью шифровать устройство.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="6b2fb-107">Дополнительные [сведения просмотрите](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) в этом документе.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="6b2fb-108">**Устройства не могут провериться в службе Intune** или отображаться как "Нездоровые" в консоли администрирования Intune: Некоторые устройства Samsung 4.4 и 5.5 могут не проверяться в службе.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="6b2fb-109">Существует 3 возможных решения этой проблемы:</span><span class="sxs-lookup"><span data-stu-id="6b2fb-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="6b2fb-110">Вручную откройте приложение Портал компании Intune, которое автоматически инициирует синхронизацию устройства.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="6b2fb-111">Обновление устройства до Android 6.0 или более.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="6b2fb-112">Отключение смарт-менеджера Samsung от управления порталом компании Intune.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="6b2fb-113">Просмотрите [этот документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для получения дополнительных сведений по этим вопросам и решениям.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="6b2fb-114">**Тип лицензии пользователя** Недействительный или имя пользователя, не распознаваемая **ошибка:** пользователю необходимо получить лицензию Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6b2fb-115">Просмотрите эти документы, чтобы назначить лицензию через: Центр администрирования Office или портал Azure.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="6b2fb-116">Дополнительные ресурсы для решения проблемы:</span><span class="sxs-lookup"><span data-stu-id="6b2fb-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6b2fb-117">Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6b2fb-118">Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="6b2fb-119">Просмотрите [этот документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) для списка распространенных ошибок, которые препятствуют регистрации и разрешений для каждого из них.</span><span class="sxs-lookup"><span data-stu-id="6b2fb-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="6b2fb-120">[Узнайте, как зарегистрироваться на устройствах Android в Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="6b2fb-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
