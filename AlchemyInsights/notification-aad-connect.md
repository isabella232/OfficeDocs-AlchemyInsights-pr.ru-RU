---
title: Уведомление AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898042"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="de4b4-102">Уведомление AAD Connect</span><span class="sxs-lookup"><span data-stu-id="de4b4-102">Notification AAD Connect</span></span>

- <span data-ttu-id="de4b4-103">Убедитесь, что вы уполномочены выполнять операцию.</span><span class="sxs-lookup"><span data-stu-id="de4b4-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="de4b4-104">Глобальные администраторы имеют доступ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="de4b4-104">Global Admins have access by default.</span></span> <span data-ttu-id="de4b4-105">Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.</span><span class="sxs-lookup"><span data-stu-id="de4b4-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="de4b4-106">Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="de4b4-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="de4b4-107">Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="de4b4-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="de4b4-108">Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.</span><span class="sxs-lookup"><span data-stu-id="de4b4-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="de4b4-109">Убедитесь, что вы проверили параметры уведомлений для Azure AD Connect Health и просмотрите параметр.</span><span class="sxs-lookup"><span data-stu-id="de4b4-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="de4b4-110">Чтобы понять, как настроить параметры уведомлений для уведомлений Azure AD Connect Health, см. в этом [руководстве.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="de4b4-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="de4b4-111">Дополнительные данные о отчете о синхронизации AAD Connect Health и его загрузке см. в отчете о синхронизации уровня [объекта.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="de4b4-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="de4b4-112">Для устранения неполадок AAD Connect Health Alerts следуйте руководству по устранению неполадок для оповещений о свежести данных [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и для часто задающихся вопросов см. в общих вопросах установки [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="de4b4-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
