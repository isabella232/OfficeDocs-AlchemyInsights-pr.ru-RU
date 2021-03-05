---
title: Проблема с AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453300"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="1e68d-102">Проблема с AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="1e68d-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="1e68d-103">Убедитесь, что вы уполномочены выполнять операцию.</span><span class="sxs-lookup"><span data-stu-id="1e68d-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="1e68d-104">Глобальные администраторы имеют доступ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1e68d-104">Global Admins have access by default.</span></span> <span data-ttu-id="1e68d-105">Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.</span><span class="sxs-lookup"><span data-stu-id="1e68d-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="1e68d-106">Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="1e68d-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="1e68d-107">Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="1e68d-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="1e68d-108">Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.</span><span class="sxs-lookup"><span data-stu-id="1e68d-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="1e68d-109">Убедитесь, что вы проверили параметры уведомлений для Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="1e68d-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="1e68d-110">Просмотрите параметр.</span><span class="sxs-lookup"><span data-stu-id="1e68d-110">Please review your setting.</span></span> <span data-ttu-id="1e68d-111">Это [руководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) поможет вам понять, как настроить параметры уведомлений для уведомлений о состоянии здоровья Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1e68d-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="1e68d-112">Дополнительные данные о отчете о синхронизации AAD Connect Health и его загрузке см. в отчете о синхронизации уровня [объекта.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="1e68d-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="1e68d-113">Чтобы устранить неполадки в оповещениях AAD Connect Health, следуйте руководству по устранению неполадок для оповещений о свежести данных [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и задайте часто задамые вопросы см. в примере Общие вопросы установки [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="1e68d-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
