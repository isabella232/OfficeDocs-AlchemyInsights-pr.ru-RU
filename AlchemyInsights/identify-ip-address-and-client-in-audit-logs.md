---
title: Определение IP-адреса и клиента в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716401"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="24705-102">Определение IP-адреса и клиента в журналах аудита</span><span class="sxs-lookup"><span data-stu-id="24705-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="24705-103">IP-адрес, соответствующий действию пользователя или администратора Microsoft 365, отображается в журналах аудита.</span><span class="sxs-lookup"><span data-stu-id="24705-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="24705-104">Сведения о клиенте также записываются в журнал.</span><span class="sxs-lookup"><span data-stu-id="24705-104">The client information is also logged.</span></span> <span data-ttu-id="24705-105">Ниже приведена процедура идентификации таких сведений.</span><span class="sxs-lookup"><span data-stu-id="24705-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="24705-106">Войдите в [центр соответствия требованиям & безопасности Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="24705-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="24705-107">Перейдите на страницу **Search** > **поиска журнала аудита** поиска.</span><span class="sxs-lookup"><span data-stu-id="24705-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="24705-108">Если вы заинтересованы в определенном действии, выберите его в списке **действия** .</span><span class="sxs-lookup"><span data-stu-id="24705-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="24705-109">В противном случае будут возвращены все действия для выбранного пользователя (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="24705-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="24705-110">**Note**: некоторые действия могут быть недоступны в меню " **действия** "; Тем не менее эти элементы аудита будут возвращены, если выбран параметр **Показать результаты для всех действий** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="24705-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="24705-111">Укажите имя пользователя в поле **Пользователи** , выберите соответствующий диапазон дат для действия и нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="24705-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="24705-112">В результатах можно просмотреть IP-адрес для этого действия в области результатов.</span><span class="sxs-lookup"><span data-stu-id="24705-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="24705-113">Выберите запись аудита, чтобы просмотреть подробные сведения в всплывающем меню **сведений** (например, клиент, пользователь, который выполнил действие и т. д.).</span><span class="sxs-lookup"><span data-stu-id="24705-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="24705-114">Для получения дополнительных сведений обратитесь к разделу [Поиск IP-адреса компьютера, используемого для доступа к скомпрометированной учетной записи](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="24705-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
