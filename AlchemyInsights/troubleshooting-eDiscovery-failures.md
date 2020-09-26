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
# <a name="troubleshoot-content-search-errors"></a>Устранение ошибок при поиске контента

Возникли ли проблемы с поиском контента или сбором сбоев при экспорте результатов поиска?

Например, при выполнении поиска вы получаете следующие сведения:

- Ошибки CS008 или CS012

- Ошибки занятости сервера/таймаута

- Ошибка приложения

Или при поиске или экспорте результатов из большого числа почтовых ящиков (свыше 100 000 почтовых ящиков) вы получаете ошибки экспорта?

Для этих типов ошибок повторите поиск расположений контента, для которых произошел сбой. Для получения дополнительных сведений обратитесь к  [этой статье](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Если вы экспортируете более 100 КБ почтовых ящиков, вам потребуется использовать следующую оболочку PowerShell, чтобы скачать результаты экспорта:  [Экспорт результатов из более чем 100 000 почтовых ящиков](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
