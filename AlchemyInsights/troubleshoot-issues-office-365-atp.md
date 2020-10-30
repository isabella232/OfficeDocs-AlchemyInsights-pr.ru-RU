---
title: Устранение проблем с защитником Microsoft для Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801420"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="8a897-102">Устранение неполадок, связанных с Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="8a897-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="8a897-103">**Задержки при доставке сообщений электронной почты** ?</span><span class="sxs-lookup"><span data-stu-id="8a897-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="8a897-104">Попробуйте использовать параметр динамической доставки для политик безопасных вложений ATP.</span><span class="sxs-lookup"><span data-stu-id="8a897-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="8a897-105">Это не позволит задержкам доставки сообщений электронной почты при защите получателей от вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="8a897-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="8a897-106">**Хотите ли вы сообщить о ложных срабатываниях или ложных отрицательные отрицательные** результаты?</span><span class="sxs-lookup"><span data-stu-id="8a897-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="8a897-107">Используйте эту ссылку, чтобы передать файл для анализа: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="8a897-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="8a897-108">**Знаете ли вы, что вы можете включить защиту для безопасных ссылок ATP для электронной почты, отправляемой между людьми в Организации** ?</span><span class="sxs-lookup"><span data-stu-id="8a897-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="8a897-109">Выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="8a897-109">Follow these steps:</span></span>
    1. <span data-ttu-id="8a897-110">Перейдите к разделу https://protection.office.com и войдите в систему.</span><span class="sxs-lookup"><span data-stu-id="8a897-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="8a897-111">Перейдите к **Threat management** разделу  >  **Policy**  >  **безопасные ссылки** политики управления угрозами.</span><span class="sxs-lookup"><span data-stu-id="8a897-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="8a897-112">В разделе **политики, которые применяются к определенным получателям** , измените (или добавьте) политику.</span><span class="sxs-lookup"><span data-stu-id="8a897-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="8a897-113">Выберите **Применить безопасные ссылки к сообщениям, отправляемым в Организации** .</span><span class="sxs-lookup"><span data-stu-id="8a897-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="8a897-114">Сохраните политику и разрешите около 30 минут, чтобы изменения работали в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="8a897-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="8a897-115">Для получения дополнительной справки по ATP обратитесь к разделу [защитник Майкрософт для Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="8a897-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>