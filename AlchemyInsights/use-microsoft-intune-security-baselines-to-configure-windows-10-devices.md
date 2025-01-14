---
title: Использование базовых конфигураций безопасности Microsoft Intune для настройки устройств с Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971532"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Использование базовых конфигураций безопасности Microsoft Intune для настройки устройств с Windows 10

Базовые конфигурации безопасности Intune помогают защитить пользователей и устройства. Базовые конфигурации безопасности — это предварительно настроенные группы параметров Windows, используемые для применения известной группы параметров и значений по умолчанию, рекомендуемых соответствующими командами безопасности. Создавая профиль базовой конфигурации безопасности в Intune, вы создаете шаблон, состоящий из нескольких профилей конфигурации устройств.

Когда вы разворачиваете базовые конфигурации безопасности для групп пользователей или устройств, эти параметры применяются к устройствам под управлением Windows 10 или более поздних версий. Например, базовая конфигурация безопасности управления мобильными устройствами (MDM) Майкрософт автоматически (1) включает BitLocker для съемных дисков, (2) требует пароля для разблокировки устройства и (3) отключает обычную проверку подлинности. Если в вашей среде не поддерживается значение по умолчанию, вы можете настроить базовую конфигурацию, чтобы применить нужные параметры.

Базовые конфигурации безопасности также помогают создать комплексный безопасный рабочий процесс в Microsoft 365. Вот некоторые преимущества этой функции:
- Базовая конфигурация безопасности включает рекомендации для параметров, влияющих на безопасность. Так как Intune взаимодействует с командой безопасности Windows, создающей базовые конфигурации для групповых политик, эти рекомендации основаны на надежных руководствах и обширном опыте.
- Если вы не работали в Intune или не знаете, с чего начать, базовые конфигурации безопасности помогут вам быстро создать и развернуть безопасный профиль.
- Если вы используете групповую политику, миграция в Intune в целях управления значительно упрощается с помощью базовых конфигураций безопасности, так как эти базовые конфигурации безопасности встроены в Intune и включают новейшие возможности управления.

Дополнительные сведения см. в статьях [Базовые конфигурации безопасности Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) и [Управление мобильными устройствами](https://docs.microsoft.com/windows/client-management/mdm/).