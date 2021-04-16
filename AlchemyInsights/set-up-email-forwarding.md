---
title: Настройка переадресации
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
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787150"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="2bfa3-102">Проверка параметров пересылания электронной почты для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="2bfa3-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="2bfa3-103">Во-первых, необходимо включить переададку электронной почты на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="2bfa3-104">Если вы настроили отправку электронной почты на почтовый ящик, но она не работает (вы получаете ошибку **"550 5.7.520** Доступ запрещен, ваша организация не разрешает внешнюю пересылку" ) см. в статью Управление автоматической внешней пересылке электронной почты в [Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="2bfa3-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="2bfa3-105">Легко проверить параметры пересылания электронной почты в почтовом ящике!</span><span class="sxs-lookup"><span data-stu-id="2bfa3-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="2bfa3-106">Просто следуйте этим шагам.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="2bfa3-107">Если это почтовый ящик пользователя, перейдите к **пользователям Users** Active и выберите пользователя, почтовый ящик которого \>  вы пересылаете.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="2bfa3-108">На **вкладке Почта** выберите **Управление пересылками электронной почты.**</span><span class="sxs-lookup"><span data-stu-id="2bfa3-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="2bfa3-109">Если это общий почтовый ящик, перейдите к общим почтовым ящикам **Groups** Shared и выберите общий почтовый ящик, который \>  вы пересылаете.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="2bfa3-110">Выберите **Изменение** для переададки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="2bfa3-111">Дополнительные сведения см. в [сообщении Configure email forwarding in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="2bfa3-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="2bfa3-112">Чтобы отправлять пользователям инструкции, чтобы они могли настроить переададку электронной почты в свои почтовые ящики, указать им переададку электронной почты из Microsoft 365 в другую учетную запись [электронной почты.](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)</span><span class="sxs-lookup"><span data-stu-id="2bfa3-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="2bfa3-113">Обратите внимание, что вы можете переададовать только один адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="2bfa3-114">Если необходимо настроить переадстройку группе людей, создайте список рассылки (в группах), добавьте к ней пользователей, а затем настроите переадпределение в эту группу.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="2bfa3-115">У вас есть сотрудник, уехав?</span><span class="sxs-lookup"><span data-stu-id="2bfa3-115">Do you have an employee leaving?</span></span> <span data-ttu-id="2bfa3-116">См. [удаление бывшего сотрудника из Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) для рекомендуемых действий.</span><span class="sxs-lookup"><span data-stu-id="2bfa3-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>