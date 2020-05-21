---
title: Необходимо пометить домен или адрес электронной почты как безопасный?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281184"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="c5969-102">Необходимо пометить домен или адрес электронной почты как безопасный?</span><span class="sxs-lookup"><span data-stu-id="c5969-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="c5969-103">**не рекомендуется использовать в списках надежных отправителей**, так как она открывает Организации в целях защиты от спама, фишинга и фишинга.</span><span class="sxs-lookup"><span data-stu-id="c5969-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="c5969-104">Однако если у вас есть деловое требование, мы **рекомендуем** использовать **[правила потока почты](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** для этого.</span><span class="sxs-lookup"><span data-stu-id="c5969-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="c5969-105">Наше руководство обеспечивает проверку подлинности отправителя (проверяет, что отправляющий домен не был подделан).</span><span class="sxs-lookup"><span data-stu-id="c5969-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="c5969-106">**Примечание**: Мы не рекомендуем управлять ложными срабатываниями с помощью списков надежных отправителей, поскольку исключения из фильтрации спама могут открыть вашу организацию для атак безопасности.</span><span class="sxs-lookup"><span data-stu-id="c5969-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="c5969-107">Если ваши пользователи получают сообщения, неправильно помеченные как спам или нежелательные сообщения, **[сообщите об этом в Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="c5969-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="c5969-108">**Следует избегать** безопасных отправителей в Outlook, списка разрешенных отправителей или списка разрешенных доменов в политиках защиты от нежелательной почты, поскольку отправители обходят все средства защиты от спама, фальсификации и фишинга, а также проверку подлинности отправителей (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="c5969-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="c5969-109">Этот метод лучше всего использовать только для временного тестирования.</span><span class="sxs-lookup"><span data-stu-id="c5969-109">This method is best used for temporary testing only.</span></span>
