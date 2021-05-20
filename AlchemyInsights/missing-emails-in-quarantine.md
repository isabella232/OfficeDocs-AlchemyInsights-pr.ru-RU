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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539837"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="f9e5c-102">Отсутствующие сообщения электронной почты в карантине"</span><span class="sxs-lookup"><span data-stu-id="f9e5c-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="f9e5c-103">Администраторы могут [просматривать, выпускать или удалять эти сообщения.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="f9e5c-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="f9e5c-104">Чтобы открыть Центр & безопасности, перейдите в [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="f9e5c-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="f9e5c-105">Чтобы открыть страницу карантина напрямую, перейдите к [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="f9e5c-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="f9e5c-106">Вы можете искать по следующим значениям:</span><span class="sxs-lookup"><span data-stu-id="f9e5c-106">You can search by the following values:</span></span>  

- <span data-ttu-id="f9e5c-107">**Идентификатор сообщения**. Глобальный уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="f9e5c-108">Если выбрать сообщение в списке, значение **ID**  сообщения появится в области сведений, которая отображается.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="f9e5c-109">Администраторы могут использовать [трассировку сообщений](/microsoft-365/security/office-365-security/message-trace-scc) для поиска сообщений и соответствующих им значений идентификатора сообщения.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="f9e5c-110">**Адрес электронной почты отправителя**: адрес электронной почты одного отправителя.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="f9e5c-111">**Адрес электронной почты получателя**: адрес электронной почты одного получателя.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="f9e5c-112">**Тема**: Используйте всю тему сообщения.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="f9e5c-113">При поиске регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="f9e5c-114">После того, как вы ввели критерии поиска, нажмите ![кнопку Обновить](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обновить**, чтобы обновить результаты.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="f9e5c-115">Для просмотра и управления сообщениями и файлами в карантине используются такие коды, как:</span><span class="sxs-lookup"><span data-stu-id="f9e5c-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="f9e5c-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f9e5c-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="f9e5c-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f9e5c-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="f9e5c-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f9e5c-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="f9e5c-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Обратите внимание, что этот комлет только для сообщений, а не файлов вредоносных программ из Microsoft Defender для Office 365 для SharePoint Online, OneDrive для бизнеса или Teams.</span><span class="sxs-lookup"><span data-stu-id="f9e5c-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="f9e5c-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f9e5c-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)