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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776094"
---
# <a name="content-search-not-returning-expected-results"></a>Поиск контента не возвращает ожидаемые результаты

При выполнении поиска по контенту из центра безопасности _Амп_ соответствия требованиям Office 365 могут возникать неожиданные результаты поиска. Обратите внимание на следующие моменты, которые могут повлиять на результаты поиска:

- **Расположения контента и условия поиска**: Убедитесь, что выбраны правильные расположения контента и условия поиска. Если вы запустили большой Поиск (с множеством расположений), рассмотрите разделение его на несколько поисков.

- **Частично индексированные элементы**: [частично индексированные элементы](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков включаются в оценочные результаты поиска. Тем не менее, частично индексированные элементы из сайтов в SharePoint и OneDrive не включаются в оценку поиска.

- **Ошибки поиска**: при поиске большого количества почтовых ящиков (свыше 100 000 почтовых ящиков) могут возникать ошибки поиска, коды ошибок, такие как CS008-009 и CS012-002). В этом случае повторите поиск только для неудачных расположений контента. Для получения дополнительных сведений обратитесь к [этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
