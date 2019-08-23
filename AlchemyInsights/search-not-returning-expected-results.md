---
title: 1491 — Поиск не возвращает ожидаемые результаты
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551428"
---
# <a name="content-search-not-returning-expected-results"></a>Поиск контента не возвращает ожидаемые результаты

При выполнении поиска контента из центра безопасности & безопасности Office 365 могут возникать неожиданные результаты поиска. Обратите внимание на следующие моменты, которые могут повлиять на результаты поиска:

- **Расположения контента и условия поиска**: Убедитесь, что выбраны правильные расположения контента и условия поиска. Если вы запустили большой Поиск (с множеством расположений), рассмотрите разделение его на несколько поисков.

- **Частично индексированные элементы**: [частично индексированные элементы](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков включаются в оценочные результаты поиска. Тем не менее, частично индексированные элементы из сайтов в SharePoint и OneDrive не включаются в оценку поиска.

- **Ошибки поиска**: при поиске большого количества почтовых ящиков (свыше 100 000 почтовых ящиков) могут возникать ошибки поиска, коды ошибок, такие как CS008-009 и CS012-002). В этом случае повторите поиск только для неудачных расположений контента. Для получения дополнительных сведений обратитесь к [этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
