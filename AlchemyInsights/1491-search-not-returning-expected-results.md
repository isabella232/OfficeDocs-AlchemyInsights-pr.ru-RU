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
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="86824-102">Не возвращает ожидаемые результаты поиска контента</span><span class="sxs-lookup"><span data-stu-id="86824-102">Content Search not returning expected results</span></span>

<span data-ttu-id="86824-p101">При выполнении операций поиска контента из & безопасности Office 365 центре соответствия требованиям, может появиться непредвиденные результаты. Рассмотрим следующие факторы, которые могут повлиять на результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="86824-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="86824-p102">**Размещения содержимого и условия поиска**: Убедитесь, что выбрано правильное размещения содержимого и условия поиска. При запуске большого поиска (с помощью различных мест), рассмотрите возможность разделения на несколько поисков.</span><span class="sxs-lookup"><span data-stu-id="86824-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="86824-p103">**Частично индексированных элементов**: [частично индексированных элементов](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков, включены в оценке результатов поиска. Тем не менее частично индексированных элементов из сайтов в SharePoint и OneDrive не включены в оценку поиска.</span><span class="sxs-lookup"><span data-stu-id="86824-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="86824-p104">**Сбои поиска**: при поиске большое число почтовых ящиков (более 100 000 почтовых ящиков), могут возникнуть ошибки поиска, с помощью кодов ошибок, таких как CS008-009 и CS012-002). В этом случае повторите попытку поиска только для неудачных размещения содержимого. [В этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="86824-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
