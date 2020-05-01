---
title: Уведомления о предупреждениях SharePoint не доставляются
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742060"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="b38bf-102">Уведомления о предупреждениях SharePoint не доставляются</span><span class="sxs-lookup"><span data-stu-id="b38bf-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="b38bf-103">Проверьте папку "Нежелательная почта" в электронной почте, как это может случиться в оповещениях.</span><span class="sxs-lookup"><span data-stu-id="b38bf-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="b38bf-104">Определите **, не доставлены ли все оповещения** или не доставлено **отдельное оповещение** из определенного файла или библиотеки.</span><span class="sxs-lookup"><span data-stu-id="b38bf-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="b38bf-105">**Индивидуальные оповещения не доставляются**: Если отдельное оповещение из определенного файла или библиотеки не доставлено, вы можете попытаться удалить его и создать повторно.</span><span class="sxs-lookup"><span data-stu-id="b38bf-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="b38bf-106">Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="b38bf-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="b38bf-107">**Все оповещения не доставляются**: Если все оповещения из нескольких файлов или библиотек не доставляются, перейдите на [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить наличие рекомендаций или инцидентов, которые могут возникнуть при работе с SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="b38bf-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="b38bf-108">Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange.</span><span class="sxs-lookup"><span data-stu-id="b38bf-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="b38bf-109">Также обратите внимание на то, что отправляются другие сообщения электронной почты, а если нет, то эта ошибка, скорее всего, связана с задержками Exchange.</span><span class="sxs-lookup"><span data-stu-id="b38bf-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="b38bf-110">Вопросы и ответы по оповещениям:</span><span class="sxs-lookup"><span data-stu-id="b38bf-110">FAQ on alerts:</span></span>

- <span data-ttu-id="b38bf-111">Невозможно отправлять оповещения в группу рассылки, поддерживаются только группы безопасности и группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="b38bf-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="b38bf-112">Вы не можете настраивать шаблоны оповещений по электронной почте; для достижения этих целей необходимо использовать Microsoft FLOW или рабочий процесс SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b38bf-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="b38bf-113">Подробнее:</span><span class="sxs-lookup"><span data-stu-id="b38bf-113">More Information:</span></span>

- <span data-ttu-id="b38bf-114">**Настройка оповещений**: Дополнительные сведения о настройке оповещений приведены [в статье Создание оповещения для получения уведомлений при изменении файлов и папок в SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="b38bf-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="b38bf-115">**Устранение неполадок оповещений**: Дополнительные сведения об устранении неполадок см. [Пользователи не получают уведомления о SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="b38bf-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="b38bf-116">**Дополнительные сведения о политиках оповещений о соответствии требованиям в O365**: Дополнительные сведения о настройке этих оповещений см. в разделе [политики оповещений о соответствии](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="b38bf-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="b38bf-117">**Журналы аудита SharePoint и OneDrive**: Дополнительные сведения о получении этих событий приведены [в статье Поиск в журнале аудита](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="b38bf-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="b38bf-118">**Оповещения, отправленные расширенной защитой от угроз**: Ознакомьтесь со статьей [ATP для SharePoint и OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="b38bf-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="b38bf-119">**Оповещения, отправляемые политиками защиты от потери данных**: просмотрите [уведомления по электронной почте для политик защиты от потери](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)данных.</span><span class="sxs-lookup"><span data-stu-id="b38bf-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="b38bf-120">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="b38bf-120">Related Topics</span></span>

<span data-ttu-id="b38bf-121">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="b38bf-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="b38bf-122">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="b38bf-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="b38bf-123">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="b38bf-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
