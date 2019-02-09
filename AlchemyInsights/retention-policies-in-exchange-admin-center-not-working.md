---
title: Политики хранения в центре администрирования Exchange не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786783"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e4516-102">Политики хранения в центре администрирования Exchange</span><span class="sxs-lookup"><span data-stu-id="e4516-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="e4516-103">**Проблема:** Вновь созданный или политики хранения обновленные в центре администрирования Exchange не применяются к почтовым ящикам или не перемещаются в архивный почтовый ящик или удалении элементов.</span><span class="sxs-lookup"><span data-stu-id="e4516-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e4516-104">**Основные причины:**</span><span class="sxs-lookup"><span data-stu-id="e4516-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="e4516-p101">Возможно, **Помощника для управляемых папок** не обработал почтовый ящик пользователя. Помощник для управляемых папок пытается обработки всех почтовых ящиков в организации на основе облака один раз в неделю. Если тега хранения или изменения другую политику хранения к почтовому ящику, подождать Assist управляемых папок обрабатывается почтовый ящик или можно запустить командлет Start-ManagedFolderAssistant запуск помощника для управляемых папок для обработки определенного почтовый ящик. Выполнение этого командлета можно использовать для проверки или устранения неполадок политику хранения или параметры тегов хранения. Для получения дополнительных сведений посетите [Запуск помощника для управляемых папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e4516-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e4516-110">**Решения:** Выполните следующую команду для запуска помощника для управляемых папок для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="e4516-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e4516-p102">Это может произойти при **RetentionHold** была **включена** для почтового ящика. Если поместил почтовый ящик на RetentionHold политики хранения для почтового ящика не будут обрабатываться в это время. Для более informaton о см параметр RetentionHold: [Удержание почтовых ящиков](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e4516-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e4516-114">**Решение:**</span><span class="sxs-lookup"><span data-stu-id="e4516-114">**Solution:**</span></span>
    
  - <span data-ttu-id="e4516-115">Проверьте состояние параметра RetentionHold на определенного почтового ящика в [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e4516-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e4516-116">Выполните следующую команду, чтобы **Отключить** RetentionHold на определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e4516-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e4516-117">Повторно запустите управляемая папка помощник по:</span><span class="sxs-lookup"><span data-stu-id="e4516-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e4516-118">**Примечание:** Если почтовый ящик меньше 10 МБ, помощника для управляемых папок не будет обрабатывать автоматически почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e4516-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

