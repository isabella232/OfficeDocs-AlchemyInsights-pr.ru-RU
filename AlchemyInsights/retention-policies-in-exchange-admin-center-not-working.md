---
title: Политики хранения в Центре администрирования Exchange не работают
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952241"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="74426-102">Политики хранения в Центре администрирования Exchange</span><span class="sxs-lookup"><span data-stu-id="74426-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="74426-103">Если вы хотите, чтобы мы запускали автоматические проверки указанных ниже параметров, выберите кнопку < -- в верхней части этой страницы, а затем введите адрес электронной почты пользователя, у которого возникли проблемы с политиками хранения.</span><span class="sxs-lookup"><span data-stu-id="74426-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="74426-104">Если у вас возникли проблемы с политиками хранения в Центре администрирования Exchange, которые не применяются к почтовым ящикам или не перемещаются в архивный почтовый ящик, проверьте следующее:</span><span class="sxs-lookup"><span data-stu-id="74426-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="74426-105">**Корневые причины:**</span><span class="sxs-lookup"><span data-stu-id="74426-105">**Root Causes:**</span></span>

- <span data-ttu-id="74426-106">**Помощник управляемой папки** не обрабатывал почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="74426-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="74426-107">Помощник управляемых папок пытается обрабатывать каждый почтовый ящик в облачной организации один раз в семь дней.</span><span class="sxs-lookup"><span data-stu-id="74426-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="74426-108">**Решение:** Запустите помощник управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="74426-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="74426-109">**Удержание** в **почтовом** ящике включено.</span><span class="sxs-lookup"><span data-stu-id="74426-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="74426-110">Если почтовый ящик размещен на удержании, политика хранения в почтовом ящике не будет обработана в течение этого времени.</span><span class="sxs-lookup"><span data-stu-id="74426-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="74426-111">**Решение:** Проверьте состояние параметра удержания хранения и обновления по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="74426-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="74426-112">Подробные сведения см. [в материале Удержание хранения почтовых ящиков.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="74426-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="74426-113">**Примечание:** Если размер почтового ящика меньше 10 МБ, помощник управляемых папок не будет автоматически обрабатывать почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="74426-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="74426-114">Дополнительные сведения о политиках хранения в Центре администрирования Exchange см. в рублях:</span><span class="sxs-lookup"><span data-stu-id="74426-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="74426-115">Теги хранения и политики хранения</span><span class="sxs-lookup"><span data-stu-id="74426-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="74426-116">[Применить политику хранения к почтовым ящикам или](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [добавить или удалить теги хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="74426-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="74426-117">Как определить тип удержания, примененного для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="74426-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
