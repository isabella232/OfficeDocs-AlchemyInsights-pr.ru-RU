---
title: Устранение неполадок, связанных с Office 365 Advanced Threat protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766758"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="6279f-102">Устранение неполадок, связанных с Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="6279f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="6279f-103">**Задержки при доставке сообщений электронной почты**?</span><span class="sxs-lookup"><span data-stu-id="6279f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="6279f-104">Попробуйте использовать параметр динамической доставки для политик безопасных вложений ATP.</span><span class="sxs-lookup"><span data-stu-id="6279f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="6279f-105">Это не позволит задержкам доставки сообщений электронной почты при защите получателей от вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="6279f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="6279f-106">**Хотите ли вы сообщить о ложных срабатываниях или ложных отрицательные отрицательные**результаты?</span><span class="sxs-lookup"><span data-stu-id="6279f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="6279f-107">Используйте эту ссылку, чтобы передать файл для анализа:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="6279f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="6279f-108">**Знаете ли вы, что вы можете включить защиту для безопасных ссылок ATP для электронной почты, отправляемой между людьми в Организации**?</span><span class="sxs-lookup"><span data-stu-id="6279f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="6279f-109">Выполните приведенные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="6279f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="6279f-110">Перейдите к https://protection.office.comразделу и войдите в систему.</span><span class="sxs-lookup"><span data-stu-id="6279f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="6279f-111">Перейдите к разделу**безопасные ссылки** > **политики** >  **управления угрозами**.</span><span class="sxs-lookup"><span data-stu-id="6279f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="6279f-112">В разделе **политики, которые применяются к определенным получателям**, измените (или добавьте) политику.</span><span class="sxs-lookup"><span data-stu-id="6279f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="6279f-113">Выберите **Применить безопасные ссылки к сообщениям, отправляемым в Организации**.</span><span class="sxs-lookup"><span data-stu-id="6279f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="6279f-114">Сохраните политику и разрешите около 30 минут, чтобы изменения работали в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="6279f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="6279f-115">Чтобы получить дополнительную справку по ATP, ознакомьтесь с разкрывающимся [пакетом Office 365 Advanced Threat protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="6279f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>