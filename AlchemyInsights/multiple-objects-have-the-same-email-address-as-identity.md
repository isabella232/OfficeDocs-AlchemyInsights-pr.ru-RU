---
title: Для нескольких объектов используется один и тот же адрес электронной почты, используемый для идентификации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724628"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="461bd-102">Для нескольких объектов используется один и тот же адрес электронной почты, используемый для идентификации</span><span class="sxs-lookup"><span data-stu-id="461bd-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="461bd-103">**Несколько объектов**</span><span class="sxs-lookup"><span data-stu-id="461bd-103">**Multiple objects**</span></span>

<span data-ttu-id="461bd-104">Одна из распространенных причин этой ошибки заключается в том, что не удается правильно маршрутизировать запрос Outlook Web Access в присутствии нескольких объектов, у которых есть один и тот же адрес электронной почты, используемый для идентификации.</span><span class="sxs-lookup"><span data-stu-id="461bd-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="461bd-105">Чтобы найти эти объекты, выполните следующие команды:</span><span class="sxs-lookup"><span data-stu-id="461bd-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="461bd-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="461bd-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="461bd-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="461bd-107">· Get-User <email address></span></span>

<span data-ttu-id="461bd-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="461bd-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="461bd-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="461bd-109">· Get-Contact <email address></span></span>

<span data-ttu-id="461bd-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="461bd-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="461bd-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="461bd-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="461bd-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="461bd-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="461bd-113">Чтобы устранить эту проблему, удалите несколько объектов с одинаковым адресом электронной почты, используемым для идентификации, и убедитесь в том, что есть один объект с определенной электронной почтой и что его типом получателя является UserMailBox.</span><span class="sxs-lookup"><span data-stu-id="461bd-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="461bd-114">\*\* Тот же адрес используется для пользовательского и корпоративного почтовых ящиков \*\*</span><span class="sxs-lookup"><span data-stu-id="461bd-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="461bd-115">Другая причина заключается в том, что один и тот же адрес используется для пользовательского и корпоративного почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="461bd-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="461bd-116">В этом случае пользователь должен изменить свой основной псевдоним пользователя до тех пор, пока Cafe не поддержит такой сценарий.</span><span class="sxs-lookup"><span data-stu-id="461bd-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="461bd-117">Это постоянная ошибка, которые не исчезает без вмешательства.</span><span class="sxs-lookup"><span data-stu-id="461bd-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="461bd-118">Дополнительные сведения см. в разделе [Изменить адрес электронной почты или номер телефона для вашей учетной записи Майкрософт](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="461bd-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>