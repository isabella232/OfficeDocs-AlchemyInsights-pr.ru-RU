---
title: Выбытие служб Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973944"
---
# <a name="access-services-retirement"></a>Выбытие служб Access

Как мы изначально объявили в MC97576, в марте 2017 и продолжали общаться в течение прошлого года службы доступа отменяются от Office 365. Следующим этапом в этом процессе будет удаление веб-баз данных Access, использующих списки SharePoint в качестве базового хранилища данных.

## <a name="how-does-this-affect-me"></a>Как это влияет на меня?

Начиная с 2019 июня мы не будем создавать новые базы данных Access в SharePoint Online, а также завершать работу службы и остальных приложений на 2020 апреля.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Что нужно сделать, чтобы подготовиться к этому изменению?

Мы рекомендуем создать план перехода для веб-баз данных доступа в Организации. Администраторы могут использовать [сканер приложения Access](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) для получения перечня приложений Access, которые используются сайтами. 

Существует несколько способов переноса данных веб-баз данных Access:

- Импорт в локальную базу данных Access (. ACCDB) или в файл Excel.
- Мы также рекомендуем изучению Microsoft PowerApps в качестве альтернативной платформы для создания бизнес-решений без кода для веб-приложений и мобильных устройств.