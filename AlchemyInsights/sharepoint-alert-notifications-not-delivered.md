---
title: Уведомления о предупреждениях SharePoint не доставляются
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751256"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="dbd15-102">Уведомления о предупреждениях SharePoint не доставляются</span><span class="sxs-lookup"><span data-stu-id="dbd15-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="dbd15-103">Проверьте папку "Нежелательная почта" в электронной почте, как это может случиться в оповещениях.</span><span class="sxs-lookup"><span data-stu-id="dbd15-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="dbd15-104">Определите **, не доставлены ли все оповещения** или не доставлено **отдельное оповещение** из определенного файла или библиотеки.</span><span class="sxs-lookup"><span data-stu-id="dbd15-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="dbd15-105">**Индивидуальные оповещения не доставляются**: Если отдельное оповещение из определенного файла или библиотеки не доставлено, вы можете попытаться удалить его и создать повторно.</span><span class="sxs-lookup"><span data-stu-id="dbd15-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="dbd15-106">Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="dbd15-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="dbd15-107">**Все оповещения не доставляются**: Если все оповещения из нескольких файлов или библиотек не доставляются, перейдите на [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить наличие рекомендаций или инцидентов, которые могут возникнуть при работе с SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbd15-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="dbd15-108">Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbd15-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="dbd15-109">Также обратите внимание на то, что отправляются другие сообщения электронной почты, а если нет, то эта ошибка, скорее всего, связана с задержками Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbd15-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="dbd15-110">Вопросы и ответы по оповещениям:</span><span class="sxs-lookup"><span data-stu-id="dbd15-110">FAQ on alerts:</span></span>

- <span data-ttu-id="dbd15-111">Невозможно отправлять оповещения в группу рассылки, поддерживаются только группы безопасности и группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="dbd15-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="dbd15-112">Вы не можете настраивать шаблоны оповещений по электронной почте; для достижения этих целей необходимо использовать Microsoft FLOW или рабочий процесс SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="dbd15-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="dbd15-113">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="dbd15-113">Related Topics</span></span>

<span data-ttu-id="dbd15-114">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="dbd15-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="dbd15-115">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="dbd15-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="dbd15-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="dbd15-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
