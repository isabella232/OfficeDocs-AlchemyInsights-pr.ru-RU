---
title: Ретрансляция почты в Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776499"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="93aba-102">Настройка многофункционального устройства или приложения для отправки электронной почты</span><span class="sxs-lookup"><span data-stu-id="93aba-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="93aba-103">Сведения о вариантах и инструкции см. в статье [Настройка многофункционального устройства или приложения для отправки электронной почты с помощью Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="93aba-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="93aba-104">**Примечание.** Если у вас есть устройство или приложение, которое недавно перестало работать, обратите внимание, что мы недавно начали [отключение шифров 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) в соответствии с планом.</span><span class="sxs-lookup"><span data-stu-id="93aba-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="93aba-105">Чтобы просмотреть затронутые устройства, откройте [Отчет о клиентах проверки подлинности SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="93aba-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="93aba-106">Примеры распространенных ошибок: сбой или ошибка при проверке подлинности, сбой или ошибка TLS, ошибка алгоритма шифрования, несоответствие алгоритмов или прерванное соединение.</span><span class="sxs-lookup"><span data-stu-id="93aba-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="93aba-107">Устранение проблемы:</span><span class="sxs-lookup"><span data-stu-id="93aba-107">To resolve the issue:</span></span>

 - <span data-ttu-id="93aba-108">**SMTP IIS Windows Server 2003 больше не будет работать — требуется более новая версия Windows.**</span><span class="sxs-lookup"><span data-stu-id="93aba-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="93aba-109">Обратитесь к поставщику приложения или устройства, чтобы узнать о поддержке современного шифрования или наличии обновлений.</span><span class="sxs-lookup"><span data-stu-id="93aba-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
