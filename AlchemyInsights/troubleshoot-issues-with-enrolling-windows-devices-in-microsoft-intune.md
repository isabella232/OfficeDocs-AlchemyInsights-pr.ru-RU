---
title: Устранение неполадок с Регистрация устройств Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486499"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="4fa6b-102">Устранение неполадок с Регистрация устройств Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4fa6b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="4fa6b-103">Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему сейчас.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4fa6b-104">Некоторые распространенные сообщения об ошибках и инструкции по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="4fa6b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="4fa6b-p101">**Не удается установить программное обеспечение, 0x80cf4017:** Истек срок действия сертификата учетной записи. Загрузите пакет программного обеспечения клиентском Компьютере в консоли администрирования Intune. Дополнительные сведения о документации.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="4fa6b-108">**Код ошибки 0x801c0003:** Ошибка может возникнуть в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="4fa6b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="4fa6b-p102">У пользователя есть несколько устройств, участвуют превышает ограничение устройства. Просмотрите эти документы, чтобы [Удалить устройство](https://docs.microsoft.com/en-us/intune/devices-wipe) или [Изменение ограничения устройства](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="4fa6b-p103">«Пользователи могут участвовать в устройствах для Azure AD» имеет значение «none». Задайте для него значение all, или выберите пользователей. Ознакомьтесь с [этой документации](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="4fa6b-p104">Устройство уже участвуют другим пользователем. Если это так, удалите его из консоли Azure Intune или вручную unenroll устройства перед повторением.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="4fa6b-p105">Устройство является 10 Windows Home. Только Windows 10 Pro, обучения и Enterprise могут присоединиться к Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="4fa6b-118">Дополнительные ресурсы, которые помогут устранить проблему:</span><span class="sxs-lookup"><span data-stu-id="4fa6b-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4fa6b-p106">[Устранение неполадок в портал Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) используйте для диагностики и устранения распространенных ошибок регистрации. Просмотрите [Этот документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="4fa6b-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4fa6b-121">Просмотрите эти документы, список распространенные ошибки, которые препятствуют регистрации и решения в каждое: [руководство по Устранение неполадок](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Устранение неполадок doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4fa6b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="4fa6b-122">[Узнайте, как возможность зачисления устройств Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="4fa6b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

