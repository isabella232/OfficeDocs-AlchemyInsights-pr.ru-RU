---
title: Выход на пенсию служб доступа
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938708"
---
# <a name="access-services-retirement"></a>Выход на пенсию служб доступа

Как мы первоначально объявили в MC97576, в марте 2017 г. и продолжали общаться в течение последнего службы Access на пенсию. Следующим этапом этого процесса будет удаление веб-баз данных Access, SharePoint списков в качестве баз данных.

**Как это влияет на меня?**

Начиная с июня 2019 г. мы прекратим создание новых баз данных access в SharePoint Online и отключим службу и все остальные приложения к апрелю 2020 г.

**Что нужно сделать, чтобы подготовиться к этому изменению?**

Мы рекомендуем вам создать план перехода для веб-баз данных Access вашей организации. Администраторы могут использовать [сканер SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для получения инвентаризации приложений Access, которые используют сайты.

Существует несколько способов переноса данных веб-баз данных Access:

- Импорт в локализованную базу данных доступа (. ACCDB) или Excel файл.
- Мы также рекомендуем Microsoft PowerApps как альтернативную платформу для создания бизнес-решений без кода для веб-устройств и мобильных устройств.