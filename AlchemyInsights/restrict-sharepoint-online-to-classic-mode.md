---
title: Ограничение SharePoint Online в классическом режиме
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958814"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Ограничение SharePoint Online в классическом режиме

Некоторые организации по-прежнему требуют классического режима. Несмотря на отсутствие планов по удалению классического режима на уровне детализации, невозможно ограничить всю организацию (клиента) классическим режимом для списков и библиотек.

Администратор будет иметь следующие параметры для управления отдельными списками и библиотеками в классическом режиме с помощью зернистых выключатели отказа, которые мы предоставляем на следующих уровнях:

- семейство веб-сайтов
- site
- список
- библиотека

Кроме того, списки с определенными функциями и настройками, не поддерживаемые современными, по-прежнему будут автоматически переключаться на классический режим.

С 1 апреля 2019 г. процесс отключения уровня клиента отключать современные списки и библиотеки начнется и продолжится до 31 мая 2019 г.  Списки и библиотеки, которые находятся в классическом режиме в результате отказа клиента, автоматически будут перенесены на современные.

Если вам требуется классический режим, см. дополнительные [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) сведения здесь и инструкция PnP Powershell здесь, где описываются параметры и средства, которые можно использовать сегодня для использования классического режима. [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)
