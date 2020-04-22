---
title: 1491 — Поиск не возвращает ожидаемые результаты
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709240"
---
# <a name="content-search-not-returning-expected-results"></a>Поиск контента не возвращает ожидаемые результаты

При выполнении поиска контента в центре безопасности & безопасности Майкрософт 365 могут возникать неожиданные результаты поиска. Обратите внимание на следующие моменты, которые могут повлиять на результаты поиска:

- **Расположения контента и условия поиска**: Убедитесь, что выбраны правильные расположения контента и условия поиска. Если вы запустили большой Поиск (с множеством расположений), рассмотрите разделение его на несколько поисков.

- **Частично индексированные элементы**: [частично индексированные элементы](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков включаются в оценочные результаты поиска. Тем не менее, частично индексированные элементы из сайтов в SharePoint и OneDrive не включаются в оценку поиска.

- **Ошибки поиска**: при поиске большого количества почтовых ящиков (свыше 100 000 почтовых ящиков) могут возникать ошибки поиска, коды ошибок, такие как CS008-009 и CS012-002). В этом случае повторите поиск только для неудачных расположений контента. Для получения дополнительных сведений обратитесь к [этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
