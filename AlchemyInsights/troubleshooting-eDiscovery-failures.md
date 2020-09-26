---
title: 1490 — устранение неполадок с обнаружением электронных данных — ошибки
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277838"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="5ee8a-102">Устранение ошибок при поиске контента</span><span class="sxs-lookup"><span data-stu-id="5ee8a-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="5ee8a-103">Возникли ли проблемы с поиском контента или сбором сбоев при экспорте результатов поиска?</span><span class="sxs-lookup"><span data-stu-id="5ee8a-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="5ee8a-104">Например, при выполнении поиска вы получаете следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="5ee8a-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="5ee8a-105">Ошибки CS008 или CS012</span><span class="sxs-lookup"><span data-stu-id="5ee8a-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="5ee8a-106">Ошибки занятости сервера/таймаута</span><span class="sxs-lookup"><span data-stu-id="5ee8a-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="5ee8a-107">Ошибка приложения</span><span class="sxs-lookup"><span data-stu-id="5ee8a-107">Application error occurred</span></span>

<span data-ttu-id="5ee8a-108">Или при поиске или экспорте результатов из большого числа почтовых ящиков (свыше 100 000 почтовых ящиков) вы получаете ошибки экспорта?</span><span class="sxs-lookup"><span data-stu-id="5ee8a-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="5ee8a-109">Для этих типов ошибок повторите поиск расположений контента, для которых произошел сбой.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="5ee8a-110">Для получения дополнительных сведений обратитесь к  [этой статье](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="5ee8a-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="5ee8a-111">Если вы экспортируете более 100 КБ почтовых ящиков, вам потребуется использовать следующую оболочку PowerShell, чтобы скачать результаты экспорта:  [Экспорт результатов из более чем 100 000 почтовых ящиков](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="5ee8a-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
