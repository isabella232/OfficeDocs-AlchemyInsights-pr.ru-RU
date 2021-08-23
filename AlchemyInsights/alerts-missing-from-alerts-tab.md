---
title: Оповещений, отсутствующих на вкладке Оповещения
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362416"
---
# <a name="alerts-missing-from-alerts-tab"></a>Оповещений, отсутствующих на вкладке Оповещения

Вкладка **Alerts** работает на основе политик установки и активации с портала управления приложениями в клиенте. Для пропуска сигналов на вкладку Оповещений также необходимо активировать вне окне политики управления **приложениями.** 

Подтверждение того, что предупреждение было сгенерировано:

1. Перейдите к политикам управления [приложениями](https://compliance.microsoft.com/m365appprotection?viewid=policies) и подтвердив, что вы создали по крайней мере одну политику Active или Audit.

1. Выберите политику, а затем выберите изменение **в** области вылетов. 

1. Проверьте конфигурацию политики, чтобы подтвердить, что оповещение должно быть сгенерировано на основе события политики, начатого более 24 часов назад.

Дополнительные сведения о оповещениях в области управления приложениями см. в приложении [Get started with app threat detection and remediation.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)