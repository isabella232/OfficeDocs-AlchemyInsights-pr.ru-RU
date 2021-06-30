---
title: Ретрансляция почты в Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117996"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="32941-102">Настройка многофункционального устройства или приложения для отправки электронной почты</span><span class="sxs-lookup"><span data-stu-id="32941-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="32941-103">Сведения о вариантах и инструкции см. в статье [Настройка многофункционального устройства или приложения для отправки электронной почты с помощью Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="32941-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="32941-104">Если у вас есть устройство или приложение, которое недавно перестало работать, наиболее распространенными проблемами являются:</span><span class="sxs-lookup"><span data-stu-id="32941-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="32941-105">**Ошибки, связанные с проверкой подлинности при использовании клиента проверки подлинности SMTP**. Мы недавно внесли изменения, связанные с работой проверки подлинности SMTP.</span><span class="sxs-lookup"><span data-stu-id="32941-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="32941-106">Дополнительные сведения об устранении проблем см. в разделе Сбой проверки подлинности в статье [Устранение проблем с принтерами, сканерами и бизнес-приложениями, отправляющими электронную почту с помощью Microsoft 365 или Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="32941-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="32941-107">**Мы поддерживаем только версию TLS 1.2 для обеспечения безопасного подключения к Office 365**. Если вы используете безопасное соединение (TLS), убедитесь, что ваше приложение или устройство поддерживает TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="32941-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="32941-108">Дополнительные сведения см. в статье [Подготовка к использованию протокола TLS 1.2 в Office 365 и Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="32941-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="32941-109">Сведения о других проблемах и способах их устранения см. в статье [Устранение проблем с принтерами, сканерами и бизнес-приложениями, отправляющими электронную почту с помощью Microsoft 365 или Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="32941-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="32941-110">Чтобы просмотреть затронутые устройства, откройте [Отчет о клиентах проверки подлинности SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="32941-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="32941-p103">**Примечание**. Exchange Online не поддерживает сценарии массовой рассылки. Чтобы массово рассылать коммерческую электронную почту (например, информационные бюллетени), необходимо использовать сторонних поставщиков, специализирующихся на этих услугах.</span><span class="sxs-lookup"><span data-stu-id="32941-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
