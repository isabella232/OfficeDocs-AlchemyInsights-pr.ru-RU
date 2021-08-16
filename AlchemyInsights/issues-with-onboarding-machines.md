---
title: Проблемы с подключением компьютеров к Microsoft Defender для конечной точки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054703"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Проблемы с подключением компьютеров к Microsoft Defender для конечной точки

У вас могут возникнуть проблемы с подключением компьютеров к службе MDE. Если у вас есть доступ к компьютеру пользователя, выполните следующие действия.

1. Скачайте последнюю предварительную версию средства диагностики [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).
2. Щелкните правой кнопкой **MDEClientAnalyzer.cmd** и выберите "Запуск от имени администратора".
3. Следуйте рекомендациям, предлагаемым в **MDEClientAnalyzer.htm**.
4. Более подробные журналы можно просмотреть в созданной вложенной папке с именем **MDEClientAnalyzerResult**.
5. Если требуется дополнительное руководство, обратитесь в [службу поддержки Microsoft Defender для конечной точки](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) и предоставьте итоговый файл MDEClientAnalyzerResult.zip для анализа.
