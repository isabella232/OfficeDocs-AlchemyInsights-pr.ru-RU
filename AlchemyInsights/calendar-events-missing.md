---
title: События календаря отсутствуют или не обновляются
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: af45345bc8779489f5e00dcaee136103e674068e29c77d8c536d012f475c33c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968716"
---
# <a name="calendar-events-missing-or-not-updating"></a>События календаря отсутствуют или не обновляются

Если элементы календаря отсутствуют или не обновляются, сначала проверьте количество элементов в свойствах папки "Календарь" в Outlook: 

1. Щелкните правой кнопкой мыши папку **Календарь** затронутого пользователя и выберите **Свойства**.

1. Выберите вкладку **Синхронизация**.

Если количество элементов в папке на сервере и автономной папке не совпадает:

1.  Выделите папку **Календарь**.

1.  Перейдите на вкладку **Отправка**/**получение** и нажмите **Обновить папку**.

Если календарь по-прежнему не обновляется или события отсутствуют, скачайте средство проверки календаря для Outlook из [Центра загрузки Майкрософт](https://www.microsoft.com/download/details.aspx?id=28786). Проверьте, содержится ли в папке календаря более 5000 элементов, так как это может вызывать проблемы, например собрания календаря не обновляются или возникают ошибки собраний. 

Дополнительные сведения см. в статье [Проблемы с производительностью Outlook при слишком большом количестве элементов или папок в кэшированном режиме файла OST или PST](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).