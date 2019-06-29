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
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355890"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="993dc-102">Поиск контента не возвращает ожидаемые результаты</span><span class="sxs-lookup"><span data-stu-id="993dc-102">Content Search not returning expected results</span></span>

<span data-ttu-id="993dc-103">При выполнении поиска контента из центра безопасности & безопасности Office 365 могут возникать неожиданные результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="993dc-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="993dc-104">Обратите внимание на следующие моменты, которые могут повлиять на результаты поиска:</span><span class="sxs-lookup"><span data-stu-id="993dc-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="993dc-105">**Расположения контента и условия поиска**: Убедитесь, что выбраны правильные расположения контента и условия поиска.</span><span class="sxs-lookup"><span data-stu-id="993dc-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="993dc-106">Если вы запустили большой Поиск (с множеством расположений), рассмотрите разделение его на несколько поисков.</span><span class="sxs-lookup"><span data-stu-id="993dc-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="993dc-107">**Частично индексированные элементы**: [частично индексированные элементы](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) из почтовых ящиков включаются в оценочные результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="993dc-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="993dc-108">Тем не менее, частично индексированные элементы из сайтов в SharePoint и OneDrive не включаются в оценку поиска.</span><span class="sxs-lookup"><span data-stu-id="993dc-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="993dc-109">**Ошибки поиска**: при поиске большого количества почтовых ящиков (свыше 100 000 почтовых ящиков) могут возникать ошибки поиска, коды ошибок, такие как CS008-009 и CS012-002).</span><span class="sxs-lookup"><span data-stu-id="993dc-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="993dc-110">В этом случае повторите поиск только для неудачных расположений контента.</span><span class="sxs-lookup"><span data-stu-id="993dc-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="993dc-111">Для получения дополнительных сведений обратитесь к [этой статье](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="993dc-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
