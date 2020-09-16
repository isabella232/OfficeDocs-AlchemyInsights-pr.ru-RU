---
title: 1336 папка RecoverableItems заполнена
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741280"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="892af-102">Папка "элементы с возможностью восстановления" заполнена</span><span class="sxs-lookup"><span data-stu-id="892af-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="892af-103">Для почтовых ящиков Exchange Online лимит хранения по умолчанию для папки "элементы с возможностью восстановления" равен 30 ГБ.</span><span class="sxs-lookup"><span data-stu-id="892af-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="892af-104">Размер хранилища для папки "элементы с возможностью восстановления" автоматически увеличивается до 100 ГБ, если почтовый ящик размещается на хранение для судебного разбирательства, удержание eDiscovery или назначается политике хранения.</span><span class="sxs-lookup"><span data-stu-id="892af-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="892af-105">Когда папка "элементы с возможностью восстановления" достигает предельного размера хранилища, функциональные возможности почтовых ящиков зависят от следующих аспектов:</span><span class="sxs-lookup"><span data-stu-id="892af-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="892af-106">Пользователь не может удалять элементы из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="892af-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="892af-107">Помощник для управляемых папок не может удалять элементы на основе тега хранения или параметров управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="892af-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="892af-108">Для почтовых ящиков с включенным восстановлением одиночных элементов или помещением на удержание процесс защиты страниц с копированием при записи не может поддерживать версии элементов, измененных пользователем.</span><span class="sxs-lookup"><span data-stu-id="892af-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="892af-109">Для почтовых ящиков, для которых включено ведение журнала аудита почтового ящика, записи журнала аудита почтовых ящиков не могут быть сохранены в подпапке audits папки "элементы с возможностью восстановления".</span><span class="sxs-lookup"><span data-stu-id="892af-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="892af-110">Для почтовых ящиков, не включенных в удержание, администраторы могут использовать `Search-Mailbox -SearchDumpsterOnly -DeleteContent` команду в Exchange Online PowerShell для удаления элементов из папки "элементы с возможностью восстановления".</span><span class="sxs-lookup"><span data-stu-id="892af-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="892af-111">Дополнительную информацию см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="892af-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="892af-112">Поиск и удаление сообщений</span><span class="sxs-lookup"><span data-stu-id="892af-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="892af-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="892af-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="892af-114">Для почтовых ящиков, находящихся на удержании, администраторам необходимо удалить удержание, прежде чем они смогут удалять элементы из папки "элементы с возможностью восстановления".</span><span class="sxs-lookup"><span data-stu-id="892af-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="892af-115">Дополнительные сведения см. в статье [Удаление элементов из папки "элементы с возможностью восстановления" в облачных почтовых ящиках на удержании](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="892af-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="892af-116">Чтобы предотвратить заполнение папки "элементы с возможностью восстановления", администраторы могут увеличить предельный размер папки "элементы с возможностью восстановления" для почтовых ящиков на хранение и настроить политику хранения почтовых ящиков, которая перемещает элементы из папки "элементы с возможностью восстановления" в архивный почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="892af-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="892af-117">[В разделе увеличение квоты элементов с возможностью восстановления для почтовых ящиков на удержании](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="892af-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
