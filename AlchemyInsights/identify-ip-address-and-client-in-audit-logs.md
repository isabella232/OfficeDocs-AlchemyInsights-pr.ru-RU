---
title: Определение IP-адреса и клиента в журналах аудита
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417024"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="14206-102">Определение IP-адреса и клиента в журналах аудита</span><span class="sxs-lookup"><span data-stu-id="14206-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="14206-103">IP-адрес, соответствующий действиям пользователя или администратора, отображается в журналах аудита.</span><span class="sxs-lookup"><span data-stu-id="14206-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="14206-104">Сведения о клиенте также записываются в журнал.</span><span class="sxs-lookup"><span data-stu-id="14206-104">The client information is also logged.</span></span> <span data-ttu-id="14206-105">Ниже приведена процедура идентификации таких сведений.</span><span class="sxs-lookup"><span data-stu-id="14206-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="14206-106">Вход в [центр соответствия требованиям _Амп_ безопасности Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="14206-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="14206-107">Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.</span><span class="sxs-lookup"><span data-stu-id="14206-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="14206-108">Если вы заинтересованы в определенном действии, выберите его в списке **действия** .</span><span class="sxs-lookup"><span data-stu-id="14206-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="14206-109">В противном случае будут возвращены все действия для выбранного пользователя (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="14206-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="14206-110">**Note**: некоторые действия могут быть недоступны в меню " **действия** "; Тем не менее эти элементы аудита будут возвращены, если выбран параметр **Показать результаты для всех действий** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="14206-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="14206-111">Укажите имя пользователя в поле **Пользователи** , выберите соответствующий диапазон дат для действия и нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="14206-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="14206-112">В результатах можно просмотреть IP-адрес для этого действия в области результатов.</span><span class="sxs-lookup"><span data-stu-id="14206-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="14206-113">Выберите запись аудита, чтобы просмотреть подробные сведения в всплывающем меню **сведений** (например, клиент, пользователь, который выполнил действие и т. д.).</span><span class="sxs-lookup"><span data-stu-id="14206-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="14206-114">Для получения дополнительных сведений обратитесь к разделу [Поиск IP-адреса компьютера, используемого для доступа к скомпрометированной учетной записи](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="14206-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
