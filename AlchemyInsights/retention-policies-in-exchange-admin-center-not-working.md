---
title: Политики хранения в центре администрирования Exchange не работают
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551356"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c966b-102">Политики хранения в центре администрирования Exchange</span><span class="sxs-lookup"><span data-stu-id="c966b-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="c966b-103">**Вопрос:** Новые или обновленные политики хранения в центре администрирования Exchange не применяются к почтовым ящикам, а элементы не перемещаются в архивный почтовый ящик или не удаляются.</span><span class="sxs-lookup"><span data-stu-id="c966b-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c966b-104">**Основные причины:**</span><span class="sxs-lookup"><span data-stu-id="c966b-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="c966b-105">Это может быть вызвано тем, что **помощник** по работе с управляемыми папками не обработал почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="c966b-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c966b-106">Помощник по работе с управляемыми папками пытается обрабатывать все почтовые ящики в облачной организации каждые семь дней.</span><span class="sxs-lookup"><span data-stu-id="c966b-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c966b-107">Если вы измените тег хранения или примените другую политику хранения к почтовому ящику, вы можете дождаться обработки почтового ящика помощником для управляемых папок или запустить командлет Start-ManagedFolderAssistant, чтобы запустить помощник по работе с управляемыми папками для обработки определенного электронной.</span><span class="sxs-lookup"><span data-stu-id="c966b-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c966b-108">Выполнение этого командлета полезно для тестирования или устранения неполадок с политикой хранения или параметрами тегов хранения.</span><span class="sxs-lookup"><span data-stu-id="c966b-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c966b-109">Для получения дополнительных сведений посетите страницу [Запуск помощника для управляемых папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c966b-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c966b-110">**Решение:** Выполните следующую команду, чтобы запустить помощник по работе с управляемыми папками для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="c966b-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c966b-111">Это также может произойти, если **ретентионхолд** был **включен** для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c966b-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c966b-112">Если почтовый ящик был включен в Ретентионхолд, политика хранения в почтовом ящике не будет обработана в течение этого времени.</span><span class="sxs-lookup"><span data-stu-id="c966b-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c966b-113">Дополнительные информатон для параметра Ретентионхолд: [удержание для хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="c966b-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c966b-114">**Решению**</span><span class="sxs-lookup"><span data-stu-id="c966b-114">**Solution:**</span></span>
    
  - <span data-ttu-id="c966b-115">Проверьте состояние параметра Ретентионхолд в определенном почтовом ящике в [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="c966b-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c966b-116">Выполните следующую команду, чтобы **Отключить** ретентионхолд для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="c966b-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c966b-117">Теперь повторно запустите помощник по работе с управляемыми папками:</span><span class="sxs-lookup"><span data-stu-id="c966b-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c966b-118">**Примечание:** Если размер почтового ящика не превышает 10 МБ, помощник по работе с управляемыми папками не будет автоматически обрабатывать этот почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="c966b-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c966b-119">Более подробную информацию о политиках хранения в центре администрирования Exchange можно узнать в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="c966b-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c966b-120">Теги хранения и политики хранения</span><span class="sxs-lookup"><span data-stu-id="c966b-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c966b-121">Применение политики хранения к почтовым ящикам</span><span class="sxs-lookup"><span data-stu-id="c966b-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c966b-122">Добавление и удаление тегов хранения</span><span class="sxs-lookup"><span data-stu-id="c966b-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c966b-123">Определение типа удержания, включенного в почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="c966b-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
