---
title: Настройка защиты от потери данных в конечной точке
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892812"
---
# <a name="configure-endpoint-dlp"></a>Настройка защиты от потери данных в конечной точке

Служба защиты от потери данных Microsoft Endpoint Protection позволяет расширить защиту и отслеживать конфиденциальную информацию на устройствах с Windows 10. После того как устройства будут интегрированы в Управление устройствами, вы сможете создавать политики защиты от потери данных. Чтобы отслеживать действия с конфиденциальными элементами, можно использовать обозреватель действий. Дополнительные сведения см. в статье [Интеграция устройств в управление устройствами](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Чтобы приступить к работе с защитой от потери данных в конечной точке:

- Убедитесь, что у вас есть соответствующая лицензия на SKU или по подписке. Дополнительные сведения см. в статье [Лицензирование SKU и по подписке](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)
- Проверьте разрешения, необходимые для управления устройствами, доступ к странице интеграции либо включите или выключите наблюдение за устройствами. Чтобы узнать больше, см. [Разрешения](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Внедрите устройства в средство управления устройствами, следуя соответствующей процедуре. Дополнительные сведения см. в статье [Интеграция устройств](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Создайте политики защиты от потери данных для защиты конфиденциальных элементов. Дополнительные сведения см. в статье [Сценарии политики защиты от потери данных в конечной точке](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Дополнительные сведения о защите от потери данных можно найти в статье [Подробнее о защите от потери данных Microsoft Endpoint в Microsoft 365 (предварительная версия)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Важные шаги сбора данных, если требуется поддержка:**

1. Скачайте [предварительную версию анализатора клиентов MDATP](https://aka.ms/betamdatpanalyzer).
1. Запустите средство от имени администратора из окна командной строки:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. При появлении запроса **Введите количество минут для сбора трассировок:** введите количество минут, необходимое для выполнения сценария.
1. Выполните сценарий

Получите выходной ZIP-файл для предоставления агенту службы поддержки.
