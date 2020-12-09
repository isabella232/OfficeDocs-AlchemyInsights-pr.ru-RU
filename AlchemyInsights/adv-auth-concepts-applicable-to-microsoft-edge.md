---
title: Дополнительные понятия проверки подлинности, применяемые к Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571892"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Дополнительные понятия проверки подлинности, применяемые к Microsoft Edge

Ниже приведены основные концепции проверки подлинности, которые относятся к Microsoft Edge:

**Упреждающий способ проверки подлинности**

При включении политики [Проактивеаусенаблед](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge будет пытаться выполнять проверку подлинности пользователей, вошедших в систему, с помощью служб Майкрософт. Через заданные промежутки времени она будет использовать веб-службу для проверки обновленного манифеста, содержащего конфигурацию для профилактической проверки подлинности.

Преимущества: упреждающее аутентификация обеспечивает проверку подлинности для ключевых служб, таких как страница новой вкладки Office. Кроме того, если служба Bing используется в качестве поисковой системы, упреждающее средство проверки подлинности повышает производительность адресной строки и помогает создавать результаты поиска, сопоставленные потребностям вашего бизнеса.

**Windows Hello Кредуи для проверки подлинности NTLM**

Если единый вход (SSO) недоступен, если веб-сайт пытается войти в систему с помощью механизма NTLM или согласования, эта функция позволит пользователю предоставлять учетные данные ОС на веб-сайте и выполнять проверку подлинности с помощью пользовательского интерфейса Windows Hello cred. Этот процесс входа будет отображаться только в Windows 10 и только для тех пользователей, которые не получают единый вход во время проверки подлинности NTLM или согласования.

**Использование сохраненных паролей для автоматического входа**

Пользователи, которые сохраняют пароли в Microsoft EDGE, могут включить автоматический вход на веб-сайты, где у них есть сохраненные учетные данные. Пользователи могут включать и отключать эту функцию в edge://settings/passwords, а также настраивать ее в политиках [диспетчера паролей](https://go.microsoft.com/fwlink/?linkid=2134622) .