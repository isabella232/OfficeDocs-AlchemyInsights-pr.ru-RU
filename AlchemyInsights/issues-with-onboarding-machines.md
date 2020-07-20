---
title: Проблемы с входящей миграцией машин
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139057"
---
# <a name="issues-with-onboarding-machines"></a>Проблемы с входящей миграцией машин

Могут возникнуть проблемы с входящей миграцией машин в службу MDATP. Если у вас есть доступ к машине пользователя, выполните следующие шаги:

1. Скачайте средство диагностики [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).
2. Извлеките и выполните MDATPAnalyzer.cmd.
3. Найдите журнал диагностики в папке MDATPClientAnalyzerResult. В эту же папку загружено средство Analyzer.
4. Просмотрите файл журнала MDATPClientAnalyzer.txt, чтобы выявить проблемы с подключением или настройками прокси-сервера интернета.