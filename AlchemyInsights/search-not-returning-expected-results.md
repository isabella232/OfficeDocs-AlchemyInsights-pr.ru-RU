---
title: 1491 — Поиск не возвращает ожидаемые результаты
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740487"
---
# <a name="content-search-not-returning-expected-results"></a>Поиск контента не возвращает ожидаемые результаты

При выполнении поиска контента в центре безопасности & безопасности Майкрософт 365 могут возникать неожиданные результаты поиска. Обратите внимание на следующие моменты, которые могут повлиять на результаты поиска:

- **Расположения контента и условия поиска**: Убедитесь, что выбраны правильные расположения контента и условия поиска. Если вы запустили большой Поиск (с множеством расположений), рассмотрите разделение его на несколько поисков.

- **Частично индексированные элементы**:  [частично индексированные элементы](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) из почтовых ящиков включаются в оценочные результаты поиска. Тем не менее, частично индексированные элементы из сайтов в SharePoint и OneDrive не включаются в оценку поиска.

- **Ошибки поиска**: при поиске большого количества почтовых ящиков (свыше 100 000 почтовых ящиков) могут возникать ошибки поиска, коды ошибок, такие как CS008-009 и CS012-002). В этом случае повторите поиск только для неудачных расположений контента. Для получения дополнительных сведений обратитесь к  [этой статье](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
