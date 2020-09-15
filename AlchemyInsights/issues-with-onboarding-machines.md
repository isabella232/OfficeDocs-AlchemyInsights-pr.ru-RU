---
title: Проблемы с входящей миграцией машин
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676895"
---
# <a name="issues-with-onboarding-machines"></a>Проблемы с входящей миграцией машин

Могут возникнуть проблемы с входящей миграцией машин в службу MDATP. Если у вас есть доступ к машине пользователя, выполните следующие шаги:

1. Скачайте средство диагностики [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).
2. Извлеките и выполните MDATPAnalyzer.cmd.
3. Найдите журнал диагностики в папке MDATPClientAnalyzerResult. В эту же папку загружено средство Analyzer.
4. Просмотрите файл журнала MDATPClientAnalyzer.txt, чтобы выявить проблемы с подключением или настройками прокси-сервера интернета.