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
# <a name="notification-aad-connect"></a>Уведомление AAD Connect

- Убедитесь, что вы уполномочены выполнять операцию. Глобальные администраторы имеют доступ по умолчанию. Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.
- Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра. Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.
- Убедитесь, что вы проверили параметры уведомлений для Azure AD Connect Health и просмотрите параметр. Чтобы понять, как настроить параметры уведомлений для уведомлений Azure AD Connect Health, см. в этом [руководстве.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Дополнительные данные о отчете о синхронизации AAD Connect Health и его загрузке см. в отчете о синхронизации уровня [объекта.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Для устранения неполадок AAD Connect Health Alerts следуйте руководству по устранению неполадок для оповещений о свежести данных [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и для часто задающихся вопросов см. в общих вопросах установки [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
