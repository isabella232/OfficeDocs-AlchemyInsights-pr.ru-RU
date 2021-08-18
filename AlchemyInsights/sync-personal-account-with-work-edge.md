---
title: Разрешение пользователю синхронизировать личную учетную запись с рабочей учетной записью в Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317291"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Разрешение пользователю синхронизировать личную учетную запись с рабочей учетной записью в Microsoft Edge

Убедитесь, что выполнены следующие условия:

- В Центре администрирования Azure Active Directory включена служба Enterprise State Roaming, для чего требуется подписка Azure Active Directory Premium или Enterprise Mobility + Security (EMS). Дополнительные сведения см. в статье [Включение Enterprise State Roaming в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable).
- Выполнено одно или оба следующих условия:
    - Для вашего клиента включена служба Azure Information Protection. Подробные сведения см. в статье [Активация зашиты Azure Rights Management из Центра администрирования Microsoft 365](https://docs.microsoft.com/azure/information-protection/activate-office365).
    - Функция Azure Active Directory Enterprise State Roaming (ESR) включена для любого пользователя или клиента. Дополнительные сведения см. в статье [Что такое Enterprise State Roaming?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview)

Если AIP и ESR отключены, сообщение об ошибке проинформирует пользователей, что для их учетных записей недоступна синхронизация.
