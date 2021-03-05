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
# <a name="problem-with-aad-connect-health"></a>Проблема с AAD Connect Health

- Убедитесь, что вы уполномочены выполнять операцию. Глобальные администраторы имеют доступ по умолчанию. Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.
- Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра. Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.
- Убедитесь, что вы проверили параметры уведомлений для Azure AD Connect Health. Просмотрите параметр. Это [руководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) поможет вам понять, как настроить параметры уведомлений для уведомлений о состоянии здоровья Azure AD Connect.
- Дополнительные данные о отчете о синхронизации AAD Connect Health и его загрузке см. в отчете о синхронизации уровня [объекта.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Чтобы устранить неполадки в оповещениях AAD Connect Health, следуйте руководству по устранению неполадок для оповещений о свежести данных [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и задайте часто задамые вопросы см. в примере Общие вопросы установки [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
