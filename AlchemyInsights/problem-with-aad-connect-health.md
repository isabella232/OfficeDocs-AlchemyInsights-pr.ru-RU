---
title: Проблема с AAD Подключение health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923765"
---
# <a name="problem-with-aad-connect-health"></a>Проблема с AAD Подключение health

- Убедитесь, что вы уполномочены выполнять операцию. Глобальные администраторы имеют доступ по умолчанию. Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.
- Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра. Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.
- Убедитесь, что вы проверили параметры уведомлений для Azure AD Подключение Health. Просмотрите параметр. В [этом](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) руководстве вы можете понять, как настроить параметры уведомлений для уведомлений Azure AD Подключение уведомлений о состоянии здоровья.
- Дополнительные данные о отчете синхронизации Подключение AAD и его загрузке см. в отчете о синхронизации [уровня](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)объектов.

Чтобы устранить неполадки в AAD Подключение health alerts, следуйте руководству по устранению неполадок для оповещений о свежести данных [AAD Подключение health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и задайте часто задамые вопросы, см. в примере Общие вопросы установки [AAD Подключение](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)health .
