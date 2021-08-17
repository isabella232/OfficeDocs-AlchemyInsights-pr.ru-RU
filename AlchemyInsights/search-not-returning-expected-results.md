---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052723"
---
# <a name="content-search-not-returning-expected-results"></a>Поиск контента, не возвращающий ожидаемые результаты

При выполнении поиска контента из центра Microsoft 365 безопасности &, вы можете получить неожиданные результаты поиска. Рассмотрим следующие вещи, которые могут повлиять на результаты поиска:

- **Расположение контента и условия поиска.** Убедитесь, что вы выбрали подходящие расположения контента и условия поиска. Если вы выполняете большой поиск (со многими расположениями), рассмотрите возможность разделения его на несколько поисков.

- **Частично индексация элементов.**  [Частично](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) индексные элементы из почтовых ящиков включены в предполагаемые результаты поиска. Однако частично индексные элементы с сайтов в SharePoint и OneDrive не включены в оценку поиска.

- Сбои **поиска.** При поиске большого количества почтовых ящиков (более 100 000 почтовых ящиков) могут возникнуть ошибки поиска с кодами ошибок, такими как CS008-009 и CS012-002). В этом случае повторное поиск только для неудались расположения контента. Дополнительные  [сведения см.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) в этой статье.
