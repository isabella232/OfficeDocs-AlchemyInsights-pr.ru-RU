---
title: Проблема с атрибутом и фильтром областей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430778"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="8df91-102">Проблема с атрибутом и фильтром областей</span><span class="sxs-lookup"><span data-stu-id="8df91-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="8df91-103">**Проблема с конфликтующими значениями UPN**</span><span class="sxs-lookup"><span data-stu-id="8df91-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="8df91-104">Подготовка пользователя из Workday в AD. При подготовке пользователя из Workday в AD отображается сообщение об ошибке **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="8df91-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="8df91-105">Не удалось выполнить операцию, так как значение имени участника-пользователя, предоставленное для добавления или изменения, не является уникальным в пределах леса.</span><span class="sxs-lookup"><span data-stu-id="8df91-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="8df91-106">Сведения об ошибке: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="8df91-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="8df91-107">Значение **userPrincipalName**, которое соединитель Workday пытается установить при создании учетной записи пользователя AD, уже существует в целевом домене AD.</span><span class="sxs-lookup"><span data-stu-id="8df91-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="8df91-108">Это означает, что (1) пользователь уже существует и не пройдена проверка совпадающего ИД для этого пользователя или (2) правило создания UPN сгенерировало конфликтующее значение.</span><span class="sxs-lookup"><span data-stu-id="8df91-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="8df91-109">Предложенные действия по решению:</span><span class="sxs-lookup"><span data-stu-id="8df91-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="8df91-110">Если пользователь уже существует и при проверке совпадающего ИД не удалось связать учетную запись Workday с учетной записью Active Directory, проверьте, одинаковы ли атрибуты совпадающих ИД (обычно **employeeID**) в Workday и AD.</span><span class="sxs-lookup"><span data-stu-id="8df91-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="8df91-111">Если они разные, проблема связана с данными и ее требуется устранить.</span><span class="sxs-lookup"><span data-stu-id="8df91-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="8df91-112">Например, если EmployeeID в Workday имеет значение 001052, а в AD — 1052, значит подсистема подготовки не сможет связать две учетные записи и попытается создать пользователя, который уже существует.</span><span class="sxs-lookup"><span data-stu-id="8df91-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="8df91-113">В этом случае решением является изменение значения **EmployeeID** в AD путем добавления нулей в начале с получением значения 001052.</span><span class="sxs-lookup"><span data-stu-id="8df91-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="8df91-114">Если выражение, создающее UPN, не создает уникальное значение, рассмотрите возможность использования функции дедупликации **SelectUniqueValue**, чтобы каждый раз создавать уникальное значение.</span><span class="sxs-lookup"><span data-stu-id="8df91-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="8df91-115">**Подготовка пользователя из Workday в AD не задает значение атрибута manager для учетной записи пользователя AD**</span><span class="sxs-lookup"><span data-stu-id="8df91-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="8df91-116">Задание подготовки пользователя из Workday в AD не задает значение атрибута **manager** для учетных записей пользователей AD.</span><span class="sxs-lookup"><span data-stu-id="8df91-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="8df91-117">Существует два возможных сценария, когда встречается такое поведение:</span><span class="sxs-lookup"><span data-stu-id="8df91-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="8df91-118">Не удается сопоставить руководителя в Workday с соответствующей учетной записью пользователя AD, так как руководитель не входит в область применения.</span><span class="sxs-lookup"><span data-stu-id="8df91-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="8df91-119">В сценарии **нескольких доменов AD** руководитель в Workday и пользователь находятся в разных доменах.</span><span class="sxs-lookup"><span data-stu-id="8df91-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="8df91-120">Попробуйте сделать следующее, чтобы устранить эту проблему:</span><span class="sxs-lookup"><span data-stu-id="8df91-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="8df91-121">Если вы определили фильтры области применения, сначала проверьте, находится ли руководитель в области и удовлетворяет ли он предложению определения области.</span><span class="sxs-lookup"><span data-stu-id="8df91-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="8df91-122">Если руководитель не удовлетворяет фильтру определения области, измените фильтр так, чтобы руководитель также находился в области применения операции подготовки.</span><span class="sxs-lookup"><span data-stu-id="8df91-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="8df91-123">Если у вас несколько доменов AD, у соединителя есть известное ограничение, связанное с невозможностью сопоставлять связи руководителей между доменами.</span><span class="sxs-lookup"><span data-stu-id="8df91-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="8df91-124">Дополнительные сведения о настройке Workday для автоматической подготовки см. в статье [Руководство по настройке Workday для автоматической подготовки пользователей](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="8df91-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













