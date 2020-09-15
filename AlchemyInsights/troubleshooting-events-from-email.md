---
title: Устранение неполадок с событиями на основе электронной почты
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658747"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="b540e-102">Устранение неполадок с событиями на основе электронной почты</span><span class="sxs-lookup"><span data-stu-id="b540e-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="b540e-103">Убедитесь, что для почтового ящика включена функция: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="b540e-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="b540e-104">Затем просмотрите журналы "События на основе электронной почты" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="b540e-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="b540e-105">В журналах "События на основе электронной почты" найдите InternetMessageId, соответствующий элементу в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b540e-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="b540e-106">TrustScore определяет, будет добавлен элемент или нет.</span><span class="sxs-lookup"><span data-stu-id="b540e-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="b540e-107">События добавляются только при условии TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="b540e-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="b540e-108">TrustScore определяется свойствами SPF, DKIM или DMARC, содержащимися в заголовке сообщения.</span><span class="sxs-lookup"><span data-stu-id="b540e-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="b540e-109">Чтобы просмотреть эти свойства:</span><span class="sxs-lookup"><span data-stu-id="b540e-109">To view these properties:</span></span>

<span data-ttu-id="b540e-110">**Классическое приложение Outlook**</span><span class="sxs-lookup"><span data-stu-id="b540e-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="b540e-111">Откройте элемент</span><span class="sxs-lookup"><span data-stu-id="b540e-111">Open the item</span></span>
- <span data-ttu-id="b540e-112">"Файл -> Свойства -> Заголовки Интернета"</span><span class="sxs-lookup"><span data-stu-id="b540e-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="b540e-113">или</span><span class="sxs-lookup"><span data-stu-id="b540e-113">or</span></span>

<span data-ttu-id="b540e-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="b540e-114">**MFCMapi**</span></span>

- <span data-ttu-id="b540e-115">Перейдите к элементу в папке "Входящие"</span><span class="sxs-lookup"><span data-stu-id="b540e-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="b540e-116">Найдите PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="b540e-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="b540e-117">Эти свойства определяются и записываются во время транспортировки и маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="b540e-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="b540e-118">Для дальнейшего устранения неполадок могут потребоваться действия по поддержке транспорта, связанные со сбоями в SPF, DKIM или DMARC.</span><span class="sxs-lookup"><span data-stu-id="b540e-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>