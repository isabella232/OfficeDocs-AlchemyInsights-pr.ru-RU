---
title: Устранение неполадок с регистрацией устройств Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708903"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d4329-102">Устранение неполадок с регистрацией устройств Windows в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d4329-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d4329-103">Просмотрите ресурсы, перечисленные ниже, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="d4329-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d4329-104">Некоторые распространенные сообщения об ошибках и действия по разрешению:</span><span class="sxs-lookup"><span data-stu-id="d4329-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d4329-105">**Программное обеспечение не может быть установлено, 0x80cf4017:** Срок действия сертификата учетной записи истек.</span><span class="sxs-lookup"><span data-stu-id="d4329-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d4329-106">Повторно скачайте пакет программного обеспечения pc Client в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="d4329-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d4329-107">Просмотрите эту документацию для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="d4329-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d4329-108">**Код ошибки 0x801c0003:** Ошибка может возникать в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="d4329-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d4329-109">У пользователя зарегистрировано больше устройств, чем лимит устройства.</span><span class="sxs-lookup"><span data-stu-id="d4329-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d4329-110">Просмотрите эти [документы, чтобы удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить ограничение устройства.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="d4329-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d4329-111">"Пользователи могут присоединяться к устройствам в Azure AD" задают "нет".</span><span class="sxs-lookup"><span data-stu-id="d4329-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d4329-112">Установите его для всех или выберите пользователей.</span><span class="sxs-lookup"><span data-stu-id="d4329-112">Set it to all or select users.</span></span> <span data-ttu-id="d4329-113">Просмотрите [эту документацию](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="d4329-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d4329-114">Устройство уже зарегистрировано другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="d4329-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d4329-115">В этом случае удалите устройство из консоли Azure Intune или снимите устройство вручную перед повторной попыткой.</span><span class="sxs-lookup"><span data-stu-id="d4329-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d4329-116">Устройство — Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="d4329-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d4329-117">Только Windows 10 Pro, Education и Enterprise SKUs могут присоединяться к Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4329-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d4329-118">Дополнительные ресурсы для решения проблемы:</span><span class="sxs-lookup"><span data-stu-id="d4329-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d4329-119">Используйте [портал устранения неполадок Intune для](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) диагностики и устранения распространенных сбоев регистрации.</span><span class="sxs-lookup"><span data-stu-id="d4329-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d4329-120">Дополнительные [сведения об](https://docs.microsoft.com/intune/help-desk-operators) этом документе.</span><span class="sxs-lookup"><span data-stu-id="d4329-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d4329-121">Ознакомьтесь со списком распространенных ошибок, связанных с регистрацией, и решениями для каждой из них в следующих документах: [Руководство по устранению неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Документация по устранению неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d4329-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d4329-122">[Узнайте, как зарегистрировать устройства Windows в Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="d4329-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
