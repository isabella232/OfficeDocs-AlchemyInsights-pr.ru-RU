---
title: Настройка службы Provision
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480756"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="5f286-102">Настройка службы Provision</span><span class="sxs-lookup"><span data-stu-id="5f286-102">Configuring the Provision service</span></span>

<span data-ttu-id="5f286-103">Для автоматического обеспечения работы с пользователем Azure AD требуются допустимые учетные данные, позволяющие подключаться к API веб-служб Workday.</span><span class="sxs-lookup"><span data-stu-id="5f286-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="5f286-104">Кроме того, кнопка "Тестовое подключение" в приложении Подготовка пользователей к AD также проверяет возможность подключения к агенту по обеспечению подключения Azure AD, связанному с доменом AD.</span><span class="sxs-lookup"><span data-stu-id="5f286-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="5f286-105">Если портал Azure возвращает ошибку при сохранении учетных данных, выполните рекомендуемые ниже действия:</span><span class="sxs-lookup"><span data-stu-id="5f286-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="5f286-106">Подтвердим, что вы настроили учетную запись пользователя системы интеграции рабочего дня, как указано в разделе Руководство Настройка пользователя системы интеграции [в Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="5f286-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="5f286-107">Подтвердите, что служба агента по обеспечению подключения к Azure AD запущена и запущена на локальном сервере Windows с помощью консоли управления службами.</span><span class="sxs-lookup"><span data-stu-id="5f286-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="5f286-108">Вы также можете проверить состояние агента на портале Azure, нажав кнопку View on-premises agents.</span><span class="sxs-lookup"><span data-stu-id="5f286-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="5f286-109">Убедитесь, что вы вводите значение для поля "Имя пользователя рабочего дня" с username@workday-имя клиента.</span><span class="sxs-lookup"><span data-stu-id="5f286-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="5f286-110">Если отсутствует имя рабочего дня-клиента, проверка подлинности рабочего дня сбой.</span><span class="sxs-lookup"><span data-stu-id="5f286-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="5f286-111">Если вы настраиваете интеграцию с клиентом реализации Workday, обратите внимание на запланированные часы простоя клиента рабочего дня.</span><span class="sxs-lookup"><span data-stu-id="5f286-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="5f286-112">Рабочий день намечено время простоя для клиентов реализации в выходные дни (как правило, с вечера пятницы по утро субботы), и сбои подключения во время этого простоя — известная проблема, которая автоматически устраняется, как только клиенты реализации вернулись в сеть.</span><span class="sxs-lookup"><span data-stu-id="5f286-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="5f286-113">В редких случаях вы также можете увидеть эту ошибку, если пароль пользователя системы интеграции изменился из-за обновления клиента или если учетная запись заблокирована или просрочена.</span><span class="sxs-lookup"><span data-stu-id="5f286-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="5f286-114">Проверьте состояние пользователя системы интеграции с администратором рабочего дня.</span><span class="sxs-lookup"><span data-stu-id="5f286-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="5f286-115">Дополнительные сведения о настройке Workday для автоматической подготовки см. в статье [Руководство по настройке Workday для автоматической подготовки пользователей](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="5f286-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
