---
title: Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391020"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c1e46-102">Устранение неполадок, связанных с регистрацией устройств с iOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c1e46-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c1e46-103">Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="c1e46-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c1e46-104">Ниже приведены наиболее распространенные сообщения об ошибках и способы их устранения.</span><span class="sxs-lookup"><span data-stu-id="c1e46-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c1e46-105">**Достигнута заглушка устройства** У пользователя больше устройств, зарегистрированных по сравнению с предельным числом устройств.</span><span class="sxs-lookup"><span data-stu-id="c1e46-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c1e46-106">Просмотрите эти документы, чтобы [удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить максимальное количество устройств](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c1e46-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c1e46-107">**Эта служба не поддерживается. Политика регистрации отсутствует:** необходимо настроить или обновить службу push-уведомлений Apple (APNs).</span><span class="sxs-lookup"><span data-stu-id="c1e46-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c1e46-108">ИзУчите [этот документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , чтобы узнать, как это сделать.</span><span class="sxs-lookup"><span data-stu-id="c1e46-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c1e46-109">**Недопустимый тип лицензии пользователя, или имя пользователя не распознано:** Пользователю необходимо назначить лицензию на Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="c1e46-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c1e46-110">Просмотрите эти документы, чтобы назначить лицензию: [центр администрирования Office](https://docs.microsoft.com/intune/licenses-assign) или [портал Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="c1e46-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c1e46-111">Дополнительные материалы по решению возникшей проблемы:</span><span class="sxs-lookup"><span data-stu-id="c1e46-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c1e46-112">Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации.</span><span class="sxs-lookup"><span data-stu-id="c1e46-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c1e46-113">Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="c1e46-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c1e46-114">Просмотрите эти документы, чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать проблемы с документацией: [руководство по устраненИю неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [Устранение неполадок документа](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c1e46-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c1e46-115">[Узнайте, как зарегистрировать устройства с iOS в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="c1e46-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

