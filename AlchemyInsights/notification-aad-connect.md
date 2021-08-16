---
title: Уведомление AAD Подключение
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097319"
---
# <a name="notification-aad-connect"></a>Уведомление AAD Подключение

- Убедитесь, что вы уполномочены выполнять операцию. Глобальные администраторы имеют доступ по умолчанию. Кроме того, вы можете использовать [управление доступом](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) на основе ролей для делегирования разрешения на регистрацию в Contributor.
- Убедитесь, что необходимые конечные точки включены и не заблокированы из-за брандмауэра. Подробнее см. в [материале "Требования".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Регистрация может привести к сбойу из-за исходящие сообщения, подвергаемой проверке SSL с помощью сетевого слоя.
- Убедитесь, что вы проверили параметры уведомлений для Azure AD Подключение и просмотрите параметр. Чтобы понять, как настроить параметры уведомлений для уведомлений Azure AD Подключение health, см. в этом [руководстве.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Дополнительные данные о отчете синхронизации Подключение AAD и его загрузке см. в отчете о синхронизации [уровня](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)объектов.

Для устранения неполадок aAD Подключение оповещения о состоянии здоровья следуете в руководстве по устранению неполадок для оповещений о свежести данных [AAD Подключение и](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) для часто задающихся вопросов см. в примере Общие вопросы установки [AAD Подключение](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)health .
