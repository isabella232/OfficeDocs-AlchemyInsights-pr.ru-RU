---
title: Устранение неполадок с регистрацией устройств iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823476"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1087e-102">Устранение неполадок с регистрацией устройств iOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1087e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1087e-103">Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="1087e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1087e-104">Некоторые распространенные сообщения об ошибках и действия по разрешению:</span><span class="sxs-lookup"><span data-stu-id="1087e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1087e-105">**Достигаемая крышка устройства** У пользователя зарегистрировано больше устройств, чем лимит устройства.</span><span class="sxs-lookup"><span data-stu-id="1087e-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1087e-106">Просмотрите эти [документы, чтобы удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить ограничение устройства.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="1087e-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1087e-107">**Эта служба не поддерживается. Нет политики регистрации:** служба push-уведомлений Apple (APNS) должна быть настроена или обновлена.</span><span class="sxs-lookup"><span data-stu-id="1087e-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="1087e-108">Просмотрите [этот документ,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) чтобы узнать, как это сделать.</span><span class="sxs-lookup"><span data-stu-id="1087e-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1087e-109">**Тип лицензии пользователя недействительный или имя пользователя не распознается:** Пользователю должна быть назначена лицензия Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="1087e-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1087e-110">Просмотрите эти документы, чтобы назначить лицензию через: [Центр администрирования Office или](https://docs.microsoft.com/intune/licenses-assign) портал [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="1087e-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1087e-111">Дополнительные ресурсы для решения проблемы:</span><span class="sxs-lookup"><span data-stu-id="1087e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1087e-112">Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации.</span><span class="sxs-lookup"><span data-stu-id="1087e-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1087e-113">Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе.</span><span class="sxs-lookup"><span data-stu-id="1087e-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1087e-114">Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1087e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1087e-115">[Узнайте, как зарегистрироваться на устройствах iOS в Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="1087e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

