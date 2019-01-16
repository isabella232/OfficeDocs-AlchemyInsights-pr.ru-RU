---
title: Папка RecoverableItems 1336 заполнен
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308346"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="d0a56-102">Папка элементов для восстановления заполнен</span><span class="sxs-lookup"><span data-stu-id="d0a56-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="d0a56-p101">Для почтовых ящиков Exchange Online в Office 365 ограничение хранилища по умолчанию для папки восстанавливаемых элементов — 30 ГБ. Ограничение хранилища для папки элементов для восстановления автоматически увеличивается до 100 ГБ, если почтовый ящик, помещенные на хранение для судебного разбирательства, удержание электронных данных или назначенной политики хранения к Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0a56-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="d0a56-105">По достижении ограничение хранилища папки элементов для восстановления функциональную возможность почтового ящика изменяется следующим образом:</span><span class="sxs-lookup"><span data-stu-id="d0a56-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="d0a56-106">Пользователь не может удалять элементы из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d0a56-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="d0a56-107">Помощник для управляемых папок не может удалять элементы на основе тега хранения или параметров управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="d0a56-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="d0a56-108">Для почтовых ящиков, которые включены восстановления одного элемента или помещенные на удержание процесс копирования при записи страницы защиты не может поддерживать версий элементов, измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="d0a56-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="d0a56-109">Для почтовых ящиков, которые имеют включено ведение журнала аудита почтовых ящиков можно сохранить нет записи журнала аудита почтовых ящиков во вложенной папке аудит в папке элементов для восстановления.</span><span class="sxs-lookup"><span data-stu-id="d0a56-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="d0a56-p102">Для почтовых ящиков, которых нет на удержание, администраторы могут использовать `Search-Mailbox -SearchDumpsterOnly -DeleteContent` в Exchange Online PowerShell, чтобы удалить элементы из папки элементов для восстановления. Дополнительные сведения в следующих разделах:</span><span class="sxs-lookup"><span data-stu-id="d0a56-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="d0a56-112">Поиск и удаление сообщений</span><span class="sxs-lookup"><span data-stu-id="d0a56-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="d0a56-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="d0a56-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="d0a56-p103">Для почтовых ящиков, которые находятся на удержании необходимо удалить удержания, прежде чем они могут удаленных элементов в папке элементов для восстановления "Администраторы". Дополнительные сведения можно [удалять элементы в папке облачные почтовые ящики на хранение элементов для восстановления](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d0a56-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="d0a56-p104">Для предотвращения папки элементов для восстановления стать полный "Администраторы" можно увеличить ограничение хранилища восстанавливаемых элементов папки для почтовых ящиков на хранение и настроить политику хранения почтового ящика, который перемещает элементы в папке элементов для восстановления архива пользователя почтовый ящик. В разделе [Увеличение квот для почтовых ящиков на хранение элементов для восстановления](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d0a56-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

