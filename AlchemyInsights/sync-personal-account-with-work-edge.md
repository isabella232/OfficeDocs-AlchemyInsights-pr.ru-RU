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
ms.openlocfilehash: 4c246fcc9ef0e3a79c3e68be491e3e7f5c6edb0b
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603283"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Разрешение пользователю синхронизировать личную учетную запись с рабочей учетной записью в Microsoft Edge

Убедитесь, что выполнены следующие условия:

- В Центре администрирования Azure Active Directory включена служба Enterprise State Roaming, для чего требуется подписка на Azure Active Directory Premium или Enterprise Mobility + Security (EMS). Дополнительные сведения см. в статье [Включение Enterprise State Roaming в Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Выполнено одно или оба следующих условия:
    - Для вашего клиента включена служба Azure Information Protection. Подробные сведения см. в статье [Активация зашиты Azure Rights Management из Центра администрирования Microsoft 365](/azure/information-protection/activate-office365).
    - Функция Azure Active Directory Enterprise State Roaming (ESR) включена для любого пользователя или клиента. Дополнительные сведения см. в статье [Что такое Enterprise State Roaming?](/azure/active-directory/devices/enterprise-state-roaming-overview)

Если AIP и ESR отключены, сообщение об ошибке проинформирует пользователей, что для их учетных записей недоступна синхронизация.
