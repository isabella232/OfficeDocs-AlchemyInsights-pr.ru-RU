---
title: Устранение неполадок, связанных с регистрацией устройств Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559674"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="bfa45-102">Устранение неполадок, связанных с регистрацией устройств Windows в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bfa45-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="bfa45-103">Просмотрите перечисленные ниже ресурсы, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="bfa45-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bfa45-104">Ниже приведены наиболее распространенные сообщения об ошибках и способы их устранения.</span><span class="sxs-lookup"><span data-stu-id="bfa45-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="bfa45-105">**Не удается установить программное обеспечение, 0x80cf4017:** Срок действия сертификата учетной записи истек.</span><span class="sxs-lookup"><span data-stu-id="bfa45-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="bfa45-106">Повторно Скачайте пакет клиентского программного обеспечения ПК в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="bfa45-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="bfa45-107">Просмотрите эту документацию, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="bfa45-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="bfa45-108">**Код ошибки 0x801c0003:** Ошибка может возникать в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="bfa45-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="bfa45-109">У пользователя больше устройств, зарегистрированных по сравнению с предельным числом устройств.</span><span class="sxs-lookup"><span data-stu-id="bfa45-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bfa45-110">Просмотрите эти документы, чтобы [удалить устройство](https://docs.microsoft.com/intune/devices-wipe) или [изменить максимальное количество устройств](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="bfa45-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="bfa45-111">Для параметра "пользователи могут присоединяться к устройствам для Azure AD" задано значение "None" (нет).</span><span class="sxs-lookup"><span data-stu-id="bfa45-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="bfa45-112">Задайте для него значение все или выберите Пользователи.</span><span class="sxs-lookup"><span data-stu-id="bfa45-112">Set it to all or select users.</span></span> <span data-ttu-id="bfa45-113">Просмотрите [эту документацию](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="bfa45-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="bfa45-114">Устройство уже зарегистрировано другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="bfa45-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="bfa45-115">В этом случае удалите устройство из консоли Azure Intune или вручную отрегистрируйте устройство, прежде чем повторять попытку.</span><span class="sxs-lookup"><span data-stu-id="bfa45-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="bfa45-116">Устройство является Windows 10 Домашняя.</span><span class="sxs-lookup"><span data-stu-id="bfa45-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="bfa45-117">Присоединиться к Azure Active Directory могут только Windows 10 профессиональная, учебные и корпоративные SKU.</span><span class="sxs-lookup"><span data-stu-id="bfa45-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="bfa45-118">Дополнительные материалы по решению возникшей проблемы:</span><span class="sxs-lookup"><span data-stu-id="bfa45-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bfa45-119">Использование [портала устранения неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) для диагностики и устранения распространенных ошибок регистрации.</span><span class="sxs-lookup"><span data-stu-id="bfa45-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bfa45-120">Просмотрите [этот документ](https://docs.microsoft.com/intune/help-desk-operators) , чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="bfa45-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bfa45-121">Просмотрите эти документы, чтобы получить список распространенных ошибок, которые не позволяют регистрироваться и разрешать проблемы с документацией: [руководство по устранению неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [Устранение неполадок документа](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bfa45-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="bfa45-122">[Узнайте, как зарегистрировать устройства Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="bfa45-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
