---
title: Отсутствующие сообщения электронной почты в карантине
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542205"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="30d43-102">Отсутствующие сообщения электронной почты в карантине "</span><span class="sxs-lookup"><span data-stu-id="30d43-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="30d43-103">Администраторы могут [просматривать, освобождать или удалять эти сообщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="30d43-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="30d43-104">Чтобы открыть центр безопасности & соответствия требованиям, перейдите на страницу [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="30d43-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="30d43-105">Чтобы напрямую открыть страницу карантина, перейдите на страницу [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="30d43-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="30d43-106">Вы можете искать по следующим значениям:</span><span class="sxs-lookup"><span data-stu-id="30d43-106">You can search by the following values:</span></span>  

- <span data-ttu-id="30d43-107">**Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d43-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="30d43-108">Если в списке выбрано сообщение, в появившейся всплывающей области **сведения** отображается значение **идентификатора сообщения** .</span><span class="sxs-lookup"><span data-stu-id="30d43-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="30d43-109">Администраторы могут использовать [трассировку сообщений](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) для поиска сообщений и соответствующих им значений идентификатора сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d43-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="30d43-110">**Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.</span><span class="sxs-lookup"><span data-stu-id="30d43-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="30d43-111">**Адрес электронной почты получателя**: адрес электронной почты одного получателя.</span><span class="sxs-lookup"><span data-stu-id="30d43-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="30d43-112">**Тема**: Используйте всю тему сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d43-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="30d43-113">При поиске регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="30d43-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="30d43-114">После ввода условий поиска нажмите кнопку ![ Обновить кнопку обновить, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** чтобы отфильтровать результаты.  </span><span class="sxs-lookup"><span data-stu-id="30d43-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="30d43-115">Для просмотра и управления сообщениями и файлами в карантине используются следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="30d43-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="30d43-116">Delete — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="30d43-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="30d43-117">Export — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="30d43-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="30d43-118">Get — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="30d43-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="30d43-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Обратите внимание, что этот командлет предназначен только для сообщений, а не от вредоносных файлов из ATP для SharePoint Online, OneDrive для бизнеса или Teams.</span><span class="sxs-lookup"><span data-stu-id="30d43-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="30d43-120">Release — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="30d43-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)