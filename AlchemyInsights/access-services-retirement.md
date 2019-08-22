---
title: Выбытие служб Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495764"
---
# <a name="access-services-retirement"></a>Выбытие служб Access

Как мы изначально объявили в MC97576, в марте 2017 и продолжали общаться в течение прошлого года службы доступа отменяются от Office 365. Следующим этапом в этом процессе будет удаление веб-баз данных Access, использующих списки SharePoint в качестве базового хранилища данных.

**Как это влияет на меня?**

Начиная с 2019 июня мы не будем создавать новые базы данных Access в SharePoint Online, а также завершать работу службы и остальных приложений на 2020 апреля.

**Что нужно сделать, чтобы подготовиться к этому изменению?**

Мы рекомендуем создать план перехода для веб-баз данных доступа в Организации. Администраторы могут использовать [сканер приложения Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для получения перечня приложений Access, которые используются сайтами.

Существует несколько способов переноса данных веб-баз данных Access:

- Импорт в локальную базу данных Access (. ACCDB) или в файл Excel.
- Мы также рекомендуем изучению Microsoft PowerApps в качестве альтернативной платформы для создания бизнес-решений без кода для веб-приложений и мобильных устройств.