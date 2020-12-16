---
title: Современный способ выставления счетов по электронной почте в Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840628"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="16436-102">Выставление счетов по электронной почте в Azure</span><span class="sxs-lookup"><span data-stu-id="16436-102">Email invoicing in Azure</span></span>

<span data-ttu-id="16436-103">Для обновления предпочтений по выставлению счетов по электронной почте нужно иметь роль владельца или участника профиля выставления счетов или учетной записи выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="16436-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="16436-104">После того как выбор сделан, все пользователи с ролями "владелец", "участник", "читатели" и "менеджер по выставлению счетов" в профиле выставления счетов получают счет по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="16436-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="16436-105">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="16436-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="16436-106">Выполните поиск по запросу **Управление затратами + выставление счетов**.</span><span class="sxs-lookup"><span data-stu-id="16436-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="16436-107">В левой части экрана выберите пункт **Счета**, а затем в верхней части страницы выберите **Счет по электронной почте**.</span><span class="sxs-lookup"><span data-stu-id="16436-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="16436-108">Если профилей выставления счетов несколько, выберите профиль выставления счетов, а затем щелкните **Включение**.</span><span class="sxs-lookup"><span data-stu-id="16436-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="16436-109">Нажмите кнопку **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="16436-109">Select **Update**.</span></span>
6. <span data-ttu-id="16436-110">Если профилей выставления счетов несколько, выберите профиль выставления счетов, а затем щелкните **Включение**.</span><span class="sxs-lookup"><span data-stu-id="16436-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="16436-111">Вы предоставляете другим пользователям доступ к просмотру, скачиванию и оплате счетов, назначая им роль менеджера по счетам для профиля выставления счетов MCA или МРА.</span><span class="sxs-lookup"><span data-stu-id="16436-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="16436-112">В случае вашего согласия на получение счета по электронной почте, пользователи также получают счет по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="16436-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="16436-113">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="16436-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="16436-114">Выполните поиск по запросу **Управление затратами + выставление счетов**.</span><span class="sxs-lookup"><span data-stu-id="16436-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="16436-115">В левой части экрана выберите **Профили выставления счетов**.</span><span class="sxs-lookup"><span data-stu-id="16436-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="16436-116">В списке профилей выставления счетов выберите профиль, для которого нужно назначить роль менеджера по выставлению счетов.</span><span class="sxs-lookup"><span data-stu-id="16436-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="16436-117">Выберите в верхней части экрана **Управление доступом (IAM)**, затем в верхней части страницы выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="16436-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="16436-118">В раскрывающемся списке "Роль" выберите **Менеджер по выставлению счетов**.</span><span class="sxs-lookup"><span data-stu-id="16436-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="16436-119">Для предоставления доступа введите адрес электронной почты учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="16436-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="16436-120">Чтобы назначить роль, нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="16436-120">Select **Save** to assign the role.</span></span>
