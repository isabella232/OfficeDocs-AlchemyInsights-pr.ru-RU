---
title: 1491-Search-NOT-returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964947"
---
# <a name="content-search-not-returning-expected-results"></a>Не возвращает ожидаемые результаты поиска контента

При выполнении операций поиска контента из & безопасности Office 365 центре соответствия требованиям, может появиться непредвиденные результаты. Рассмотрим следующие факторы, которые могут повлиять на результаты поиска.

- **Размещения содержимого и условия поиска**: Убедитесь, что выбрано правильное размещения содержимого и условия поиска. При запуске большого поиска (с помощью различных мест), рассмотрите возможность разделения на несколько поисков.

- **Частично индексированных элементов**: [частично индексированных элементов](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков, включены в оценке результатов поиска. Тем не менее частично индексированных элементов из сайтов в SharePoint и OneDrive не включены в оценку поиска.

- **Сбои поиска**: при поиске большое число почтовых ящиков (более 100 000 почтовых ящиков), могут возникнуть ошибки поиска, с помощью кодов ошибок, таких как CS008-009 и CS012-002). В этом случае повторите попытку поиска только для неудачных размещения содержимого. [В этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) для получения дополнительных сведений см.
