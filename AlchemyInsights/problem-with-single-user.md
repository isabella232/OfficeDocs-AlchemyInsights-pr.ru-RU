---
title: Проблема с одним пользователем
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428828"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="ae487-102">Проблема с одним пользователем</span><span class="sxs-lookup"><span data-stu-id="ae487-102">Problem with single user</span></span>

- <span data-ttu-id="ae487-103">Возможно, пользователь не был готов, так как у службы еще не было возможности оценить пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae487-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="ae487-104">Просмотрите инструкции по длительному обеспечению, а также планку прогресса на странице конфигурации подготовка.</span><span class="sxs-lookup"><span data-stu-id="ae487-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="ae487-105">Если стабильное состояние, указанное в разделе дополнительные сведения, находится до даты создания или обновления или удаления пользователя, это означает, что мы еще не оценили пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae487-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="ae487-106">В этом сценарии лучше всего дождаться завершения службы подготовка.</span><span class="sxs-lookup"><span data-stu-id="ae487-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="ae487-107">Обратите внимание, что наша служба знает об изменениях только для пользователя в исходных системах (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="ae487-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="ae487-108">Для обнаружения изменения и потока его в Active Directory в системе исходных данных Azure AD необходимо изменить допустимые изменения.</span><span class="sxs-lookup"><span data-stu-id="ae487-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="ae487-109">Служба предварительной оценки пользователя и определила, что она не должна быть предварительной:</span><span class="sxs-lookup"><span data-stu-id="ae487-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="ae487-110">Если вы установили фильтр scoping на основе атрибутов, убедитесь, что пользователь соответствует указанным критериям.</span><span class="sxs-lookup"><span data-stu-id="ae487-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="ae487-111">Если пользователи уже существуют в целевой системе и состояние пользователя в совпадении источника и цели, мы не будем принимать никаких дальнейших действий.</span><span class="sxs-lookup"><span data-stu-id="ae487-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="ae487-112">Служба предварительного обеспечения попыталась про условии предоставления пользователю, и она не удалась.</span><span class="sxs-lookup"><span data-stu-id="ae487-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="ae487-113">В этих сценариях просмотрите вкладку устранения неполадок и рекомендации журналов подготовка:</span><span class="sxs-lookup"><span data-stu-id="ae487-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="ae487-114">Необходимый атрибут пользователя может быть пропущен в локальном каталоге Active Directory или Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae487-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ae487-115">Например, правила генерации userPrincipalName или sAMAccountName не генерируют нужное значение.</span><span class="sxs-lookup"><span data-stu-id="ae487-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="ae487-116">Соответствие атрибуту (обычно employeeId) не является решением для уникального пользователя в локальном Active Directory или Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae487-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ae487-117">Например, в AD есть два пользователя с одним и тем же сотрудникомId, и служба возвращает код ошибки, указывающий дублировать целевые записи для одной и той же начальной записи.</span><span class="sxs-lookup"><span data-stu-id="ae487-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="ae487-118">Чтобы просмотреть журналы для одного пользователя и групп, см. в обзоре журналов предварительной записи для проблемы [с определенным пользователем.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="ae487-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
