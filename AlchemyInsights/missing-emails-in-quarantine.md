---
title: Отсутствующие сообщения электронной почты в карантине
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831747"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="d8236-102">Отсутствующие сообщения электронной почты в карантине"</span><span class="sxs-lookup"><span data-stu-id="d8236-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="d8236-103">Администраторы могут [просматривать, выпускать или удалять эти сообщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="d8236-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="d8236-104">Чтобы открыть Центр & безопасности, перейдите в [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="d8236-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="d8236-105">Чтобы открыть страницу карантина напрямую, перейдите к [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="d8236-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="d8236-106">Вы можете искать по следующим значениям:</span><span class="sxs-lookup"><span data-stu-id="d8236-106">You can search by the following values:</span></span>  

- <span data-ttu-id="d8236-107">**Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="d8236-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="d8236-108">Если выбрать сообщение в списке, значение **ID**  сообщения появится в области сведений, которая отображается.</span><span class="sxs-lookup"><span data-stu-id="d8236-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="d8236-109">Администраторы могут использовать [трассировку сообщений](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) для поиска сообщений и соответствующих им значений идентификатора сообщения.</span><span class="sxs-lookup"><span data-stu-id="d8236-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="d8236-110">**Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.</span><span class="sxs-lookup"><span data-stu-id="d8236-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="d8236-111">**Адрес электронной почты получателя**: адрес электронной почты одного получателя.</span><span class="sxs-lookup"><span data-stu-id="d8236-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="d8236-112">**Тема**: Используйте всю тему сообщения.</span><span class="sxs-lookup"><span data-stu-id="d8236-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="d8236-113">При поиске регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="d8236-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="d8236-114">После того как вы ввели критерии поиска, нажмите кнопку ![ Обновить ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **обновление,** чтобы отфильтровать результаты.  </span><span class="sxs-lookup"><span data-stu-id="d8236-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="d8236-115">Для просмотра и управления сообщениями и файлами в карантине используются такие коды, как:</span><span class="sxs-lookup"><span data-stu-id="d8236-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="d8236-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d8236-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="d8236-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d8236-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="d8236-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d8236-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="d8236-119">[Preview-QuarantineMessage.](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обратите внимание, что этот командлет только для сообщений, а не файлов вредоносных программ из ATP для SharePoint Online, OneDrive для бизнеса или Teams.</span><span class="sxs-lookup"><span data-stu-id="d8236-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="d8236-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d8236-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)