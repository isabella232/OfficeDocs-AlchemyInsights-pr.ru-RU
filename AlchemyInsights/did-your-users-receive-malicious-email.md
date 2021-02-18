---
title: Ваши пользователи получили вредоносное сообщение электронной почты?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291805"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="6545d-102">Ваши пользователи получили вредоносное сообщение электронной почты?</span><span class="sxs-lookup"><span data-stu-id="6545d-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="6545d-103">Теперь вы можете сообщить о вредоносном сообщении в корпорацию Майкрософт с помощью [Отправки администратора в Центре безопасности и соответствия требованиям](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="6545d-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="6545d-104">Сообщения, отправленные с помощью [отправки администратора](https://sip.protection.office.com/reportsubmission), и во всплывающем окне **сведений** отображаются следующие результаты:</span><span class="sxs-lookup"><span data-stu-id="6545d-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="6545d-105">Возникновение сбоя при проверке подлинности электронной почты отправителя в момент доставки.</span><span class="sxs-lookup"><span data-stu-id="6545d-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="6545d-106">Сведения о любых совпадениях политик, которые могут повлиять на решение по безопасности касательно сообщения или переопределить его.</span><span class="sxs-lookup"><span data-stu-id="6545d-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="6545d-107">Текущие результаты отключения, чтобы определить, были ли URL-адреса или файлы, содержащиеся в сообщении, вредоносными или нет.</span><span class="sxs-lookup"><span data-stu-id="6545d-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="6545d-108">Отзывы оценщиков</span><span class="sxs-lookup"><span data-stu-id="6545d-108">Feedback from graders</span></span>

<span data-ttu-id="6545d-109">Если было обнаружено переопределение, повторное сканирование должно завершиться через несколько минут.</span><span class="sxs-lookup"><span data-stu-id="6545d-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="6545d-110">Если проблема не связана с проверкой подлинности электронной почты или переопределение не повлияло на доставку, то обратная связь оценщиков может занять до суток.</span><span class="sxs-lookup"><span data-stu-id="6545d-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="6545d-111">Если вы не согласны с конечным решением по безопасности касательно сообщения, URL-адреса или файла (заблокированных или не заблокированных), отправьте сообщение через день после повторного сканирования.</span><span class="sxs-lookup"><span data-stu-id="6545d-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="6545d-112">Очень высокая вероятность того, что решение по безопасности изменится после повторной отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="6545d-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="6545d-113">В то же время вы можете удалить вредоносную электронную почту из пользовательских папок "Входящие", следуя инструкциям, в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="6545d-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="6545d-114">Пользователи с Microsoft Defender для Office 365 могут:</span><span class="sxs-lookup"><span data-stu-id="6545d-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="6545d-115">использовать [обозреватель угроз для поиска и удаления подозрительных сообщений электронной почты](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="6545d-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="6545d-116">[использовать Безопасные ссылки, чтобы заблокировать доступ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) к вредоносному URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="6545d-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="6545d-117">отслеживать пользователей, нажимавших на вредоносные URL-адреса и получивших к ним доступ. [Просмотр фишингового URL-адреса и нажатие на сведенья о решении по безопасности](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Получение-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="6545d-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="6545d-118">вручную [начать автоматическое исследование](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="6545d-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="6545d-119">Также вы можете создать защиту от вредоносных файлов и URL-адресов, следуя инструкциям в статье [Защита от вредоносных URL-адресов и файлов](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="6545d-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>