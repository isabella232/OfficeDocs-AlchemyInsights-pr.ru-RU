---
title: Ретрансляция почты в Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 727fa38233697c778caa9325b2671501cb75d5fd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510729"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="3979d-102">Настройка многофункционального устройства или приложения для отправки электронной почты</span><span class="sxs-lookup"><span data-stu-id="3979d-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="3979d-103">Сведения о вариантах и инструкции см. в статье [Настройка многофункционального устройства или приложения для отправки электронной почты с помощью Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="3979d-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="3979d-104">**Примечание.** Если у вас есть устройство или приложение, которое недавно перестало работать, обратите внимание, что мы недавно начали [отключение шифров 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) в соответствии с планом.</span><span class="sxs-lookup"><span data-stu-id="3979d-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="3979d-105">Чтобы просмотреть затронутые устройства, откройте [Отчет о клиентах проверки подлинности SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3979d-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="3979d-106">Примеры распространенных ошибок: сбой или ошибка при проверке подлинности, сбой или ошибка TLS, ошибка алгоритма шифрования, несоответствие алгоритмов или прерванное соединение.</span><span class="sxs-lookup"><span data-stu-id="3979d-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="3979d-107">Устранение проблемы:</span><span class="sxs-lookup"><span data-stu-id="3979d-107">To resolve the issue:</span></span>
 - <span data-ttu-id="3979d-108">**SMTP IIS Windows Server 2003 больше не будет работать — требуется более новая версия Windows.**</span><span class="sxs-lookup"><span data-stu-id="3979d-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="3979d-109">Обратитесь к поставщику приложения или устройства, чтобы узнать о поддержке современного шифрования или наличии обновлений.</span><span class="sxs-lookup"><span data-stu-id="3979d-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
