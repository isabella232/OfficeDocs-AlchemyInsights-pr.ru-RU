---
title: Используйте Microsoft Intune безопасности для настройки Windows 10 устройств
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104357"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Используйте Microsoft Intune безопасности для настройки Windows 10 устройств

Базовые конфигурации безопасности Intune помогают защитить пользователей и устройства. Базовые конфигурации безопасности — это предварительно настроенные группы параметров Windows, используемые для применения известной группы параметров и значений по умолчанию, рекомендуемых соответствующими командами безопасности. Создавая профиль базовой конфигурации безопасности в Intune, вы создаете шаблон, состоящий из нескольких профилей конфигурации устройств.

При развертывании базовых показателей безопасности для групп пользователей или устройств эти параметры применяются к устройствам, которые работают на Windows 10 или позже. Например, базовый уровень безопасности MDM автоматически (1) включает BitLocker для съемных дисков, (2) требует пароль для разблокировки устройства, а (3) отключает базовую проверку подлинности. Если значение по умолчанию не работает для среды, настройте базовый уровень, чтобы применить необходимые параметры.

Базовые конфигурации безопасности также помогают создать комплексный безопасный рабочий процесс в Microsoft 365. Ниже приводится ряд преимуществ:

- Базовая конфигурация безопасности включает рекомендации для параметров, влияющих на безопасность. Так как Intune взаимодействует с командой безопасности Windows, создающей базовые конфигурации для групповых политик, эти рекомендации основаны на надежных руководствах и обширном опыте.
- Если вы не работали в Intune или не знаете, с чего начать, базовые конфигурации безопасности помогут вам быстро создать и развернуть безопасный профиль.
- Если вы в настоящее время используете групповую политику, то перейти в Intune в целях управления намного проще с базовыми показателями безопасности, так как они встроены в Intune и включают передовые возможности управления.

Дополнительные данные см. [в Windows базовых показателей](https://go.microsoft.com/fwlink/?linkid=2141503) безопасности и [управления мобильными устройствами.](https://go.microsoft.com/fwlink/?linkid=2141701)